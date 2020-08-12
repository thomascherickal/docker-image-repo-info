<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.6`](#consul16)
-	[`consul:1.6.8`](#consul168)
-	[`consul:1.7`](#consul17)
-	[`consul:1.7.7`](#consul177)
-	[`consul:1.8`](#consul18)
-	[`consul:1.8.3`](#consul183)
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

## `consul:1.6.8`

**does not exist** (yet?)

## `consul:1.7`

```console
$ docker pull consul@sha256:523fb793b8240853d395138142f9f4bf329dc72b2e11ca8891726c9fa30cafa7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7` - linux; amd64

```console
$ docker pull consul@sha256:134914a56539ef1c702f9177554a5358ccf08beba1eb53dc0951c59ed124b2d6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.5 MB (43472291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e450b525e8747f0ad0e48e4839c590cd67505a103b374ab3e42b21f6c4ad7d41`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 07 Aug 2020 23:19:56 GMT
ENV CONSUL_VERSION=1.7.6
# Fri, 07 Aug 2020 23:19:56 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 07 Aug 2020 23:19:57 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 07 Aug 2020 23:20:01 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 07 Aug 2020 23:20:02 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 07 Aug 2020 23:20:03 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 23:20:03 GMT
VOLUME [/consul/data]
# Fri, 07 Aug 2020 23:20:03 GMT
EXPOSE 8300
# Fri, 07 Aug 2020 23:20:03 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 07 Aug 2020 23:20:04 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 07 Aug 2020 23:20:04 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 07 Aug 2020 23:20:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Aug 2020 23:20:04 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab1090b721ed2eec9ecff7b5da8fc508d0af8b80cf7ee51c91eeab940c4998d`  
		Last Modified: Fri, 07 Aug 2020 23:20:28 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d712999a58942dce6bfe229cd568a372b6f2347fde670171cb145479f8a850c`  
		Last Modified: Fri, 07 Aug 2020 23:20:34 GMT  
		Size: 40.7 MB (40671515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b60d3c63c3690449310d618d5c01b2ea34c9c1686fd4efe4fe02b7b744e4d7c9`  
		Last Modified: Fri, 07 Aug 2020 23:20:28 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b53b62c87b220542b0752ef7766d05933998fa0cd99b21b28b10ff620f9bce3`  
		Last Modified: Fri, 07 Aug 2020 23:20:27 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926935d2a98f38e3ddc4861579e3bfc29dc3bc6ac56e7271dd1e7b58656912a8`  
		Last Modified: Fri, 07 Aug 2020 23:20:28 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm variant v6

```console
$ docker pull consul@sha256:30728e95547749ca541cf97b204a687e89186cda741bba31b18803e111b45945
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39159295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5c5a081849d5dd564fd708421b2ff16d913597daf3df2eb06068399fadc60e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:49:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 07 Aug 2020 23:50:26 GMT
ENV CONSUL_VERSION=1.7.6
# Fri, 07 Aug 2020 23:50:27 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 07 Aug 2020 23:50:31 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 07 Aug 2020 23:51:18 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 07 Aug 2020 23:52:20 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 07 Aug 2020 23:53:42 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 23:54:08 GMT
VOLUME [/consul/data]
# Fri, 07 Aug 2020 23:54:34 GMT
EXPOSE 8300
# Fri, 07 Aug 2020 23:55:04 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 07 Aug 2020 23:55:25 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 07 Aug 2020 23:55:47 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 07 Aug 2020 23:56:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Aug 2020 23:56:20 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517e9bfed15e08ebbdc9d3abab773b5425725cec3af967fa3cd41bbd0b612702`  
		Last Modified: Fri, 07 Aug 2020 23:57:23 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42887c00ef7ab81315bc1362fd2529e6a92bd14447ec9bd4e8406338791f0218`  
		Last Modified: Fri, 07 Aug 2020 23:57:32 GMT  
		Size: 36.6 MB (36552711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a3de07b874e410cadd793d115e16ad6e12135dfb741e02ddcd0f25b0bb8d93`  
		Last Modified: Fri, 07 Aug 2020 23:57:23 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3454899120fcfa3f8a35ddb02f3579e66e22ecab6b86528eb29c382fd3838579`  
		Last Modified: Fri, 07 Aug 2020 23:57:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebce269c996333f2f7fcfe2def22c2437ce134a73b71b6daef428b80b5dba97f`  
		Last Modified: Fri, 07 Aug 2020 23:57:24 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:bef5ea242dee984ab666b75555b0b34bf0fb9cfc2bcfdd26e12fe2a082ce0e92
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.4 MB (39390906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff97e89fce84c455f67b68a150de7fb727c182827b78b8b3655881f657f3af3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:42:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 07 Aug 2020 23:40:42 GMT
ENV CONSUL_VERSION=1.7.6
# Fri, 07 Aug 2020 23:40:42 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 07 Aug 2020 23:40:44 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 07 Aug 2020 23:40:50 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 07 Aug 2020 23:40:53 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 07 Aug 2020 23:40:54 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 23:40:55 GMT
VOLUME [/consul/data]
# Fri, 07 Aug 2020 23:40:56 GMT
EXPOSE 8300
# Fri, 07 Aug 2020 23:40:56 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 07 Aug 2020 23:40:57 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 07 Aug 2020 23:40:57 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 07 Aug 2020 23:40:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Aug 2020 23:40:59 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053a4a20c0459cb94515dca8276bbcb1809a595b0becff1d2dc4179825cd46e5`  
		Last Modified: Fri, 07 Aug 2020 23:41:36 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30fc9644e15b438712f285b352f820f481946e710d1e5f6218b9adbb775aa296`  
		Last Modified: Fri, 07 Aug 2020 23:41:47 GMT  
		Size: 36.7 MB (36679646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594d3cde71dff9c0358f132796012d60b72dfcbdc048e154bf09998c886bb4b8`  
		Last Modified: Fri, 07 Aug 2020 23:41:36 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec198af636e631de7b1ba95c85040a1908ee372eea713d2eeb033309f4b4941d`  
		Last Modified: Fri, 07 Aug 2020 23:41:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599db3405d218191d1bab78a0abf4ad7c0abdb90a13da749b7b7d7444ab36beb`  
		Last Modified: Fri, 07 Aug 2020 23:41:35 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; 386

```console
$ docker pull consul@sha256:21fb38a0e203d3511f19ace2caffc3e1d827b5c300a3f5db0f71136c8c87168a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42262249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27dfc16c1250c7c12c8f25ea00c650b77aa443d231d4ef14d640af2a06bcdbda`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:38:31 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 07 Aug 2020 23:38:43 GMT
ENV CONSUL_VERSION=1.7.6
# Fri, 07 Aug 2020 23:38:43 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 07 Aug 2020 23:38:44 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 07 Aug 2020 23:38:50 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 07 Aug 2020 23:38:51 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 07 Aug 2020 23:38:52 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 23:38:52 GMT
VOLUME [/consul/data]
# Fri, 07 Aug 2020 23:38:52 GMT
EXPOSE 8300
# Fri, 07 Aug 2020 23:38:52 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 07 Aug 2020 23:38:52 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 07 Aug 2020 23:38:53 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 07 Aug 2020 23:38:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Aug 2020 23:38:53 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfb20ef751c82d580853eda1975cbca4003dfcb6affa0cd2813f61b01fb696c`  
		Last Modified: Fri, 07 Aug 2020 23:39:20 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a0138bbfe8402277f09b205dcdb41011040ca10395b7c21af84d5d8c361492`  
		Last Modified: Fri, 07 Aug 2020 23:39:27 GMT  
		Size: 39.5 MB (39466715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5508ee68f72f0b056ad5f01bd636e5428551f3f9c12acc764ca4513b5f179ba6`  
		Last Modified: Fri, 07 Aug 2020 23:39:21 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700c24e7424bfefeb49c10e9d53636089ae068b8aad4756ba73a0c4f0db19ad7`  
		Last Modified: Fri, 07 Aug 2020 23:39:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d872d2e5a55d613d697246081659d8514e47b6ea7c187e71efdaa2182d2debf1`  
		Last Modified: Fri, 07 Aug 2020 23:39:20 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7.7`

**does not exist** (yet?)

## `consul:1.8`

```console
$ docker pull consul@sha256:539a85ebc1e83bc76f6f3cfde6c7a1e8a3a4d46fcbd824de44ccfd3f6f82415a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8` - linux; amd64

```console
$ docker pull consul@sha256:201b0075ed8a7b351207ceb535ad7d5c91696c281b21addf85027b76b9278ac2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46704891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45f9911e51f6e38982e8a4ed9a575f00402210ca67ba232e1e39e358cdda874f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 07 Aug 2020 23:19:44 GMT
ENV CONSUL_VERSION=1.8.2
# Fri, 07 Aug 2020 23:19:44 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 07 Aug 2020 23:19:45 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 07 Aug 2020 23:19:49 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 07 Aug 2020 23:19:50 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 07 Aug 2020 23:19:51 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 23:19:51 GMT
VOLUME [/consul/data]
# Fri, 07 Aug 2020 23:19:51 GMT
EXPOSE 8300
# Fri, 07 Aug 2020 23:19:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 07 Aug 2020 23:19:52 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 07 Aug 2020 23:19:52 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 07 Aug 2020 23:19:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Aug 2020 23:19:52 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e25b90332b5e6b5331f7cccca0f3b4ea912995ddcca7197c06d8c9e4f53fdc`  
		Last Modified: Fri, 07 Aug 2020 23:20:16 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471863178ef7153f10a8ccb3df88198fabe278d8022e3734540a1814090c1850`  
		Last Modified: Fri, 07 Aug 2020 23:20:23 GMT  
		Size: 43.9 MB (43904115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1669621deaf9e9f8fb5ebabdc4f798ccda31b868cc2876f5eff38c3bfbffed`  
		Last Modified: Fri, 07 Aug 2020 23:20:16 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac021cc7402d99b45d0d53d4bd314bed64beb3a352450bac3d846a3e8e508a50`  
		Last Modified: Fri, 07 Aug 2020 23:20:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3069bfce7b28e9f1bf546cd3a54108a6925336a73f0b434e7e57cfbdee96d8b`  
		Last Modified: Fri, 07 Aug 2020 23:20:16 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm variant v6

```console
$ docker pull consul@sha256:236050f020b8723e098a8fdb6b019867f399bc45e4255c085bafca5af561aca2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41989355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b58214a005e0194048329b07726cf23621cbc92a77b940ef714f1686ad1a7803`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:49:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 07 Aug 2020 23:49:35 GMT
ENV CONSUL_VERSION=1.8.2
# Fri, 07 Aug 2020 23:49:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 07 Aug 2020 23:49:43 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 07 Aug 2020 23:50:04 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 07 Aug 2020 23:50:07 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 07 Aug 2020 23:50:12 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 23:50:13 GMT
VOLUME [/consul/data]
# Fri, 07 Aug 2020 23:50:13 GMT
EXPOSE 8300
# Fri, 07 Aug 2020 23:50:14 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 07 Aug 2020 23:50:14 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 07 Aug 2020 23:50:16 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 07 Aug 2020 23:50:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Aug 2020 23:50:18 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6db771b44502823f9dcca700cf77f8081f19a3fb5f03589bea86f6e7c39019`  
		Last Modified: Fri, 07 Aug 2020 23:56:51 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb14eba257dd6dadd1830b367f7282295d154cc6204232144efa95a616957ddd`  
		Last Modified: Fri, 07 Aug 2020 23:57:08 GMT  
		Size: 39.4 MB (39382776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79639c4315dac8ec3f82fbc23c6681ae0e7b28c9f415108053030b9f927ec813`  
		Last Modified: Fri, 07 Aug 2020 23:56:51 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26213e3033758dc9a67778a246be1bcda7edb4062e38816bf2ee65ffde36baff`  
		Last Modified: Fri, 07 Aug 2020 23:56:51 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fd2b442821ec1ead7b13fde4067ca29d65e047e3192adca0b8070d5a627ad7`  
		Last Modified: Fri, 07 Aug 2020 23:56:51 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:a59da069f3f289c88c5ac39a66d23da8b1c6d540290a919677ef4bf41505f4d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.2 MB (42154084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76baed9c6e7f5d349b6f980e68cb5fc61ed954ac02d4ce56324faea94e956d55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:42:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 07 Aug 2020 23:40:11 GMT
ENV CONSUL_VERSION=1.8.2
# Fri, 07 Aug 2020 23:40:13 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 07 Aug 2020 23:40:15 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 07 Aug 2020 23:40:22 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 07 Aug 2020 23:40:24 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 07 Aug 2020 23:40:26 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 23:40:27 GMT
VOLUME [/consul/data]
# Fri, 07 Aug 2020 23:40:27 GMT
EXPOSE 8300
# Fri, 07 Aug 2020 23:40:28 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 07 Aug 2020 23:40:29 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 07 Aug 2020 23:40:29 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 07 Aug 2020 23:40:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Aug 2020 23:40:31 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7759389d712d34deabecb07bb6623359c775f38eb3ec23c1c255389667fdca5e`  
		Last Modified: Fri, 07 Aug 2020 23:41:17 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3400e3d210da07d9a078f64c5ab56f654a222fbcb4e39314fb1e2ce9f4a4fe4b`  
		Last Modified: Fri, 07 Aug 2020 23:41:27 GMT  
		Size: 39.4 MB (39442825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573ce4b45093e20fa89259bb2c54e1fafcde0e2480160bbbd7ff49e39829aa6a`  
		Last Modified: Fri, 07 Aug 2020 23:41:17 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b1ed0125348b8a8aaad457be16fd084804fc8ccb9e48129f5cc332c8a18e49`  
		Last Modified: Fri, 07 Aug 2020 23:41:17 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5d66d10bc907a2958d1b293303277c5bfa73087a77fce3753970ec80675012`  
		Last Modified: Fri, 07 Aug 2020 23:41:17 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; 386

```console
$ docker pull consul@sha256:8d0f56105cd2499857edeef0a39085a99852d5483487a48c3119d941f80a3f96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46219422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95d60e0832a305d9ac4aa5d84d6ba9aea55bab5a207c0a3ac4faeaf3c1e99930`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:38:31 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 07 Aug 2020 23:38:29 GMT
ENV CONSUL_VERSION=1.8.2
# Fri, 07 Aug 2020 23:38:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 07 Aug 2020 23:38:30 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 07 Aug 2020 23:38:36 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 07 Aug 2020 23:38:36 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 07 Aug 2020 23:38:37 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 23:38:38 GMT
VOLUME [/consul/data]
# Fri, 07 Aug 2020 23:38:38 GMT
EXPOSE 8300
# Fri, 07 Aug 2020 23:38:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 07 Aug 2020 23:38:38 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 07 Aug 2020 23:38:38 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 07 Aug 2020 23:38:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Aug 2020 23:38:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007f5c49b9a7ff5ba06c41e57896df44b84453ea47a87e49a258210f958b5e5d`  
		Last Modified: Fri, 07 Aug 2020 23:39:08 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7cfe4b71b3c7d500237542f2a202ff12defa48bc5b44957ccd038675022046d`  
		Last Modified: Fri, 07 Aug 2020 23:39:16 GMT  
		Size: 43.4 MB (43423887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49944b87fefb975a33c6fc89a3064cca6d27f8e4694ab0cb2451eae8fc8fdde3`  
		Last Modified: Fri, 07 Aug 2020 23:39:08 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369a2b6a1e3b2cd12514f5c997a3c2a07f97b399a04c2d9a5ad9e4ca07e2b734`  
		Last Modified: Fri, 07 Aug 2020 23:39:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1f8988d37e7803627df5d57881d37b17809984e369a35c582fb588c76f496e`  
		Last Modified: Fri, 07 Aug 2020 23:39:08 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8.3`

**does not exist** (yet?)

## `consul:latest`

```console
$ docker pull consul@sha256:539a85ebc1e83bc76f6f3cfde6c7a1e8a3a4d46fcbd824de44ccfd3f6f82415a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:201b0075ed8a7b351207ceb535ad7d5c91696c281b21addf85027b76b9278ac2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46704891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45f9911e51f6e38982e8a4ed9a575f00402210ca67ba232e1e39e358cdda874f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 07 Aug 2020 23:19:44 GMT
ENV CONSUL_VERSION=1.8.2
# Fri, 07 Aug 2020 23:19:44 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 07 Aug 2020 23:19:45 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 07 Aug 2020 23:19:49 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 07 Aug 2020 23:19:50 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 07 Aug 2020 23:19:51 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 23:19:51 GMT
VOLUME [/consul/data]
# Fri, 07 Aug 2020 23:19:51 GMT
EXPOSE 8300
# Fri, 07 Aug 2020 23:19:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 07 Aug 2020 23:19:52 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 07 Aug 2020 23:19:52 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 07 Aug 2020 23:19:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Aug 2020 23:19:52 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e25b90332b5e6b5331f7cccca0f3b4ea912995ddcca7197c06d8c9e4f53fdc`  
		Last Modified: Fri, 07 Aug 2020 23:20:16 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471863178ef7153f10a8ccb3df88198fabe278d8022e3734540a1814090c1850`  
		Last Modified: Fri, 07 Aug 2020 23:20:23 GMT  
		Size: 43.9 MB (43904115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1669621deaf9e9f8fb5ebabdc4f798ccda31b868cc2876f5eff38c3bfbffed`  
		Last Modified: Fri, 07 Aug 2020 23:20:16 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac021cc7402d99b45d0d53d4bd314bed64beb3a352450bac3d846a3e8e508a50`  
		Last Modified: Fri, 07 Aug 2020 23:20:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3069bfce7b28e9f1bf546cd3a54108a6925336a73f0b434e7e57cfbdee96d8b`  
		Last Modified: Fri, 07 Aug 2020 23:20:16 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:236050f020b8723e098a8fdb6b019867f399bc45e4255c085bafca5af561aca2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41989355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b58214a005e0194048329b07726cf23621cbc92a77b940ef714f1686ad1a7803`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:49:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 07 Aug 2020 23:49:35 GMT
ENV CONSUL_VERSION=1.8.2
# Fri, 07 Aug 2020 23:49:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 07 Aug 2020 23:49:43 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 07 Aug 2020 23:50:04 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 07 Aug 2020 23:50:07 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 07 Aug 2020 23:50:12 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 23:50:13 GMT
VOLUME [/consul/data]
# Fri, 07 Aug 2020 23:50:13 GMT
EXPOSE 8300
# Fri, 07 Aug 2020 23:50:14 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 07 Aug 2020 23:50:14 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 07 Aug 2020 23:50:16 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 07 Aug 2020 23:50:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Aug 2020 23:50:18 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6db771b44502823f9dcca700cf77f8081f19a3fb5f03589bea86f6e7c39019`  
		Last Modified: Fri, 07 Aug 2020 23:56:51 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb14eba257dd6dadd1830b367f7282295d154cc6204232144efa95a616957ddd`  
		Last Modified: Fri, 07 Aug 2020 23:57:08 GMT  
		Size: 39.4 MB (39382776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79639c4315dac8ec3f82fbc23c6681ae0e7b28c9f415108053030b9f927ec813`  
		Last Modified: Fri, 07 Aug 2020 23:56:51 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26213e3033758dc9a67778a246be1bcda7edb4062e38816bf2ee65ffde36baff`  
		Last Modified: Fri, 07 Aug 2020 23:56:51 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fd2b442821ec1ead7b13fde4067ca29d65e047e3192adca0b8070d5a627ad7`  
		Last Modified: Fri, 07 Aug 2020 23:56:51 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:a59da069f3f289c88c5ac39a66d23da8b1c6d540290a919677ef4bf41505f4d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.2 MB (42154084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76baed9c6e7f5d349b6f980e68cb5fc61ed954ac02d4ce56324faea94e956d55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:42:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 07 Aug 2020 23:40:11 GMT
ENV CONSUL_VERSION=1.8.2
# Fri, 07 Aug 2020 23:40:13 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 07 Aug 2020 23:40:15 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 07 Aug 2020 23:40:22 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 07 Aug 2020 23:40:24 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 07 Aug 2020 23:40:26 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 23:40:27 GMT
VOLUME [/consul/data]
# Fri, 07 Aug 2020 23:40:27 GMT
EXPOSE 8300
# Fri, 07 Aug 2020 23:40:28 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 07 Aug 2020 23:40:29 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 07 Aug 2020 23:40:29 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 07 Aug 2020 23:40:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Aug 2020 23:40:31 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7759389d712d34deabecb07bb6623359c775f38eb3ec23c1c255389667fdca5e`  
		Last Modified: Fri, 07 Aug 2020 23:41:17 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3400e3d210da07d9a078f64c5ab56f654a222fbcb4e39314fb1e2ce9f4a4fe4b`  
		Last Modified: Fri, 07 Aug 2020 23:41:27 GMT  
		Size: 39.4 MB (39442825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573ce4b45093e20fa89259bb2c54e1fafcde0e2480160bbbd7ff49e39829aa6a`  
		Last Modified: Fri, 07 Aug 2020 23:41:17 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b1ed0125348b8a8aaad457be16fd084804fc8ccb9e48129f5cc332c8a18e49`  
		Last Modified: Fri, 07 Aug 2020 23:41:17 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5d66d10bc907a2958d1b293303277c5bfa73087a77fce3753970ec80675012`  
		Last Modified: Fri, 07 Aug 2020 23:41:17 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:8d0f56105cd2499857edeef0a39085a99852d5483487a48c3119d941f80a3f96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46219422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95d60e0832a305d9ac4aa5d84d6ba9aea55bab5a207c0a3ac4faeaf3c1e99930`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:38:31 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 07 Aug 2020 23:38:29 GMT
ENV CONSUL_VERSION=1.8.2
# Fri, 07 Aug 2020 23:38:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 07 Aug 2020 23:38:30 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 07 Aug 2020 23:38:36 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 07 Aug 2020 23:38:36 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 07 Aug 2020 23:38:37 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 23:38:38 GMT
VOLUME [/consul/data]
# Fri, 07 Aug 2020 23:38:38 GMT
EXPOSE 8300
# Fri, 07 Aug 2020 23:38:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 07 Aug 2020 23:38:38 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 07 Aug 2020 23:38:38 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 07 Aug 2020 23:38:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Aug 2020 23:38:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007f5c49b9a7ff5ba06c41e57896df44b84453ea47a87e49a258210f958b5e5d`  
		Last Modified: Fri, 07 Aug 2020 23:39:08 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7cfe4b71b3c7d500237542f2a202ff12defa48bc5b44957ccd038675022046d`  
		Last Modified: Fri, 07 Aug 2020 23:39:16 GMT  
		Size: 43.4 MB (43423887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49944b87fefb975a33c6fc89a3064cca6d27f8e4694ab0cb2451eae8fc8fdde3`  
		Last Modified: Fri, 07 Aug 2020 23:39:08 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369a2b6a1e3b2cd12514f5c997a3c2a07f97b399a04c2d9a5ad9e4ca07e2b734`  
		Last Modified: Fri, 07 Aug 2020 23:39:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1f8988d37e7803627df5d57881d37b17809984e369a35c582fb588c76f496e`  
		Last Modified: Fri, 07 Aug 2020 23:39:08 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
