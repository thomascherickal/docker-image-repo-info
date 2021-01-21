<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.7`](#consul17)
-	[`consul:1.7.11`](#consul1711)
-	[`consul:1.8`](#consul18)
-	[`consul:1.8.7`](#consul187)
-	[`consul:1.9`](#consul19)
-	[`consul:1.9.2`](#consul192)
-	[`consul:latest`](#consullatest)

## `consul:1.7`

```console
$ docker pull consul@sha256:d3489079ba913bbe7d3cc4686b73c787f0a8de361eeea1fca4de34ce5260216c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7` - linux; amd64

```console
$ docker pull consul@sha256:d3683601dd9cc20cd4969fac363116222e833265a83d776fd5d33e1d6f965456
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43112089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0e0eba50d3b049948667de2d39eaf9373ddc9c3d1592d43b2ffdda0323c727`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:01:24 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 17 Dec 2020 13:02:09 GMT
ENV CONSUL_VERSION=1.7.11
# Thu, 17 Dec 2020 13:02:09 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Dec 2020 13:02:11 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Dec 2020 13:02:17 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Dec 2020 13:02:18 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Dec 2020 13:02:19 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:02:20 GMT
VOLUME [/consul/data]
# Thu, 17 Dec 2020 13:02:20 GMT
EXPOSE 8300
# Thu, 17 Dec 2020 13:02:20 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Dec 2020 13:02:20 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Dec 2020 13:02:21 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Dec 2020 13:02:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:02:22 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38622a0158719d6de8ffcc5817f82c0b4f7512e9b99cebcff830a70e388d4caa`  
		Last Modified: Thu, 17 Dec 2020 13:03:14 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d97316584422042e1243f7009b90eb44c42e2c316fe948b06903fa9f544f3cf`  
		Last Modified: Thu, 17 Dec 2020 13:03:22 GMT  
		Size: 40.3 MB (40309787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0f00a35b11d6923f895b64293804b63ef10c0d5a61bc77bc98bedce028fd67`  
		Last Modified: Thu, 17 Dec 2020 13:03:14 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2b7ef38504511feeac67554f6ebc6cdde14a07809ec6f80270a572a8d9a108`  
		Last Modified: Thu, 17 Dec 2020 13:03:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c86827a282a46c1b1cb3b4391ee29451d27f5646e11e0b895eb9744c559902`  
		Last Modified: Thu, 17 Dec 2020 13:03:14 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm variant v6

```console
$ docker pull consul@sha256:05ee41541bb8a82cf0520576c2f7259a85558d78f043a1d24024df6d71129635
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38814558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c53db86118b4c03987e46ebd9fa6fc02b1205f3bb0f0a20b742dd556b343887c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:15:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 17 Dec 2020 01:17:00 GMT
ENV CONSUL_VERSION=1.7.11
# Thu, 17 Dec 2020 01:17:01 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Dec 2020 01:17:04 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Dec 2020 01:17:13 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Dec 2020 01:17:19 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Dec 2020 01:17:22 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:17:23 GMT
VOLUME [/consul/data]
# Thu, 17 Dec 2020 01:17:24 GMT
EXPOSE 8300
# Thu, 17 Dec 2020 01:17:26 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Dec 2020 01:17:27 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Dec 2020 01:17:28 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Dec 2020 01:17:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:17:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c30331eb99cb51ffca2aa2a8fd8ad621e84f12d2e969783c199c85ff10aa68b`  
		Last Modified: Thu, 17 Dec 2020 01:18:41 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6e62223d40a09a1032e5fe51ba2724bdc81997490dfd79db59bc4c0948ce78a`  
		Last Modified: Thu, 17 Dec 2020 01:18:51 GMT  
		Size: 36.2 MB (36207099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ce345d054b03b6e3d4a30a186e784c4ad13c66b1253262d636103ede912e71`  
		Last Modified: Thu, 17 Dec 2020 01:18:42 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851ad82f5b67d1aef02fa57123d93e105d6d774f0c9fe5b9a53e315b9d1f71df`  
		Last Modified: Thu, 17 Dec 2020 01:18:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751bd51851908004a062198c6d551fc029e85c561e587b9224a3e1af15873dd7`  
		Last Modified: Thu, 17 Dec 2020 01:18:42 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:41516bc3582f07f44efac634d84696f96d63218a4c8ca6d7ea122a5a67b9ca3f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (39023099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0effff3a634c1ed468f236e6dd586ccb439475af4bc1c808fd6af61353e07add`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:36:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 17 Dec 2020 00:37:46 GMT
ENV CONSUL_VERSION=1.7.11
# Thu, 17 Dec 2020 00:37:46 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Dec 2020 00:37:49 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Dec 2020 00:37:59 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Dec 2020 00:38:02 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Dec 2020 00:38:04 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 00:38:04 GMT
VOLUME [/consul/data]
# Thu, 17 Dec 2020 00:38:05 GMT
EXPOSE 8300
# Thu, 17 Dec 2020 00:38:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Dec 2020 00:38:06 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Dec 2020 00:38:07 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Dec 2020 00:38:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 00:38:08 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867f35d7fa00f4c32ce6fe2ae77b396e64d1e8e33c511ad06fdc6be931a55749`  
		Last Modified: Thu, 17 Dec 2020 00:39:07 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b56e3302ccabc9a53f441a5179a1a1578f34a3e6a869b5c37d2525b5d5a7d7`  
		Last Modified: Thu, 17 Dec 2020 00:39:16 GMT  
		Size: 36.3 MB (36310761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4697c1fe65af51b748a8a21de7deb99ccfadfed3b184f8efbc385f4feb383f`  
		Last Modified: Thu, 17 Dec 2020 00:39:07 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3063fc22520d9966309e9ba656492a1b19678e707b769e6595f5dc27bf539b68`  
		Last Modified: Thu, 17 Dec 2020 00:39:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8304d79d0e0c256f2bd5ba4a9ab441cf1671ff75317e28b530fe28c5c65540`  
		Last Modified: Thu, 17 Dec 2020 00:39:07 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; 386

```console
$ docker pull consul@sha256:9885dc3f979fbe26ff497901cf66b146cb598e83072f9766e7d7747b7278c727
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41900731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1c2cb4b2059f15cb4d370d6541dd02d7f585298315f2a846cf7387a62d49af4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:24:05 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 17 Dec 2020 01:24:41 GMT
ENV CONSUL_VERSION=1.7.11
# Thu, 17 Dec 2020 01:24:41 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Dec 2020 01:24:42 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Dec 2020 01:24:49 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Dec 2020 01:24:51 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Dec 2020 01:24:52 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:24:52 GMT
VOLUME [/consul/data]
# Thu, 17 Dec 2020 01:24:53 GMT
EXPOSE 8300
# Thu, 17 Dec 2020 01:24:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Dec 2020 01:24:54 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Dec 2020 01:24:54 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Dec 2020 01:24:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:24:55 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57825a694bf08e12d5521cfca8938ad16cfe3ff39f1b8a75076668d8a4b4f1c0`  
		Last Modified: Thu, 17 Dec 2020 01:25:52 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642fb04c0d71504c45d4d985f29b19de8d52633d37982023d8b5f2cc5f9e7afd`  
		Last Modified: Thu, 17 Dec 2020 01:26:00 GMT  
		Size: 39.1 MB (39103366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b30c7ca46875a57e80bafb10176257128b44945cb7a61f7ecada53a2a8ebce`  
		Last Modified: Thu, 17 Dec 2020 01:25:52 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cfd06565bf9a9ac539063c6e1e8f184230c97ff6b7d133137aa235b2d70184`  
		Last Modified: Thu, 17 Dec 2020 01:25:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d9b39a7efd70694948768d2db1745c73205ad3cc9d87db3d235f5a3f557fbd`  
		Last Modified: Thu, 17 Dec 2020 01:25:52 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7.11`

```console
$ docker pull consul@sha256:d3489079ba913bbe7d3cc4686b73c787f0a8de361eeea1fca4de34ce5260216c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7.11` - linux; amd64

```console
$ docker pull consul@sha256:d3683601dd9cc20cd4969fac363116222e833265a83d776fd5d33e1d6f965456
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43112089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0e0eba50d3b049948667de2d39eaf9373ddc9c3d1592d43b2ffdda0323c727`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:01:24 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 17 Dec 2020 13:02:09 GMT
ENV CONSUL_VERSION=1.7.11
# Thu, 17 Dec 2020 13:02:09 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Dec 2020 13:02:11 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Dec 2020 13:02:17 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Dec 2020 13:02:18 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Dec 2020 13:02:19 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:02:20 GMT
VOLUME [/consul/data]
# Thu, 17 Dec 2020 13:02:20 GMT
EXPOSE 8300
# Thu, 17 Dec 2020 13:02:20 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Dec 2020 13:02:20 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Dec 2020 13:02:21 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Dec 2020 13:02:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:02:22 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38622a0158719d6de8ffcc5817f82c0b4f7512e9b99cebcff830a70e388d4caa`  
		Last Modified: Thu, 17 Dec 2020 13:03:14 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d97316584422042e1243f7009b90eb44c42e2c316fe948b06903fa9f544f3cf`  
		Last Modified: Thu, 17 Dec 2020 13:03:22 GMT  
		Size: 40.3 MB (40309787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0f00a35b11d6923f895b64293804b63ef10c0d5a61bc77bc98bedce028fd67`  
		Last Modified: Thu, 17 Dec 2020 13:03:14 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2b7ef38504511feeac67554f6ebc6cdde14a07809ec6f80270a572a8d9a108`  
		Last Modified: Thu, 17 Dec 2020 13:03:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c86827a282a46c1b1cb3b4391ee29451d27f5646e11e0b895eb9744c559902`  
		Last Modified: Thu, 17 Dec 2020 13:03:14 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.11` - linux; arm variant v6

```console
$ docker pull consul@sha256:05ee41541bb8a82cf0520576c2f7259a85558d78f043a1d24024df6d71129635
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38814558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c53db86118b4c03987e46ebd9fa6fc02b1205f3bb0f0a20b742dd556b343887c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:15:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 17 Dec 2020 01:17:00 GMT
ENV CONSUL_VERSION=1.7.11
# Thu, 17 Dec 2020 01:17:01 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Dec 2020 01:17:04 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Dec 2020 01:17:13 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Dec 2020 01:17:19 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Dec 2020 01:17:22 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:17:23 GMT
VOLUME [/consul/data]
# Thu, 17 Dec 2020 01:17:24 GMT
EXPOSE 8300
# Thu, 17 Dec 2020 01:17:26 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Dec 2020 01:17:27 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Dec 2020 01:17:28 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Dec 2020 01:17:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:17:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c30331eb99cb51ffca2aa2a8fd8ad621e84f12d2e969783c199c85ff10aa68b`  
		Last Modified: Thu, 17 Dec 2020 01:18:41 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6e62223d40a09a1032e5fe51ba2724bdc81997490dfd79db59bc4c0948ce78a`  
		Last Modified: Thu, 17 Dec 2020 01:18:51 GMT  
		Size: 36.2 MB (36207099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ce345d054b03b6e3d4a30a186e784c4ad13c66b1253262d636103ede912e71`  
		Last Modified: Thu, 17 Dec 2020 01:18:42 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851ad82f5b67d1aef02fa57123d93e105d6d774f0c9fe5b9a53e315b9d1f71df`  
		Last Modified: Thu, 17 Dec 2020 01:18:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751bd51851908004a062198c6d551fc029e85c561e587b9224a3e1af15873dd7`  
		Last Modified: Thu, 17 Dec 2020 01:18:42 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.11` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:41516bc3582f07f44efac634d84696f96d63218a4c8ca6d7ea122a5a67b9ca3f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (39023099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0effff3a634c1ed468f236e6dd586ccb439475af4bc1c808fd6af61353e07add`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:36:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 17 Dec 2020 00:37:46 GMT
ENV CONSUL_VERSION=1.7.11
# Thu, 17 Dec 2020 00:37:46 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Dec 2020 00:37:49 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Dec 2020 00:37:59 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Dec 2020 00:38:02 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Dec 2020 00:38:04 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 00:38:04 GMT
VOLUME [/consul/data]
# Thu, 17 Dec 2020 00:38:05 GMT
EXPOSE 8300
# Thu, 17 Dec 2020 00:38:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Dec 2020 00:38:06 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Dec 2020 00:38:07 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Dec 2020 00:38:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 00:38:08 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867f35d7fa00f4c32ce6fe2ae77b396e64d1e8e33c511ad06fdc6be931a55749`  
		Last Modified: Thu, 17 Dec 2020 00:39:07 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b56e3302ccabc9a53f441a5179a1a1578f34a3e6a869b5c37d2525b5d5a7d7`  
		Last Modified: Thu, 17 Dec 2020 00:39:16 GMT  
		Size: 36.3 MB (36310761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4697c1fe65af51b748a8a21de7deb99ccfadfed3b184f8efbc385f4feb383f`  
		Last Modified: Thu, 17 Dec 2020 00:39:07 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3063fc22520d9966309e9ba656492a1b19678e707b769e6595f5dc27bf539b68`  
		Last Modified: Thu, 17 Dec 2020 00:39:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8304d79d0e0c256f2bd5ba4a9ab441cf1671ff75317e28b530fe28c5c65540`  
		Last Modified: Thu, 17 Dec 2020 00:39:07 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.11` - linux; 386

```console
$ docker pull consul@sha256:9885dc3f979fbe26ff497901cf66b146cb598e83072f9766e7d7747b7278c727
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41900731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1c2cb4b2059f15cb4d370d6541dd02d7f585298315f2a846cf7387a62d49af4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:24:05 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 17 Dec 2020 01:24:41 GMT
ENV CONSUL_VERSION=1.7.11
# Thu, 17 Dec 2020 01:24:41 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Dec 2020 01:24:42 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Dec 2020 01:24:49 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Dec 2020 01:24:51 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Dec 2020 01:24:52 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:24:52 GMT
VOLUME [/consul/data]
# Thu, 17 Dec 2020 01:24:53 GMT
EXPOSE 8300
# Thu, 17 Dec 2020 01:24:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Dec 2020 01:24:54 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Dec 2020 01:24:54 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Dec 2020 01:24:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:24:55 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57825a694bf08e12d5521cfca8938ad16cfe3ff39f1b8a75076668d8a4b4f1c0`  
		Last Modified: Thu, 17 Dec 2020 01:25:52 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642fb04c0d71504c45d4d985f29b19de8d52633d37982023d8b5f2cc5f9e7afd`  
		Last Modified: Thu, 17 Dec 2020 01:26:00 GMT  
		Size: 39.1 MB (39103366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b30c7ca46875a57e80bafb10176257128b44945cb7a61f7ecada53a2a8ebce`  
		Last Modified: Thu, 17 Dec 2020 01:25:52 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cfd06565bf9a9ac539063c6e1e8f184230c97ff6b7d133137aa235b2d70184`  
		Last Modified: Thu, 17 Dec 2020 01:25:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d9b39a7efd70694948768d2db1745c73205ad3cc9d87db3d235f5a3f557fbd`  
		Last Modified: Thu, 17 Dec 2020 01:25:52 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8`

```console
$ docker pull consul@sha256:8530be78726dda04dac948a1a707af92af524a76091f42e7da2a7d90dd7ccd1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8` - linux; amd64

```console
$ docker pull consul@sha256:eb610ada2181c939654a24803ed28c6eb12afaa728abbf9c44065d10b65c18a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46492534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:811fe376f2881e483cc66f4faf9391f8193ca4620244580af0deb5e0b8238c70`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:01:24 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 17 Dec 2020 13:01:47 GMT
ENV CONSUL_VERSION=1.8.7
# Thu, 17 Dec 2020 13:01:47 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Dec 2020 13:01:49 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Dec 2020 13:01:57 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Dec 2020 13:01:59 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Dec 2020 13:02:00 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:02:01 GMT
VOLUME [/consul/data]
# Thu, 17 Dec 2020 13:02:01 GMT
EXPOSE 8300
# Thu, 17 Dec 2020 13:02:01 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Dec 2020 13:02:02 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Dec 2020 13:02:02 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Dec 2020 13:02:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:02:03 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbaaa36fc2fbe94736d643e90c21a848a00d3d50f9670cc18c0f4abeca674b2`  
		Last Modified: Thu, 17 Dec 2020 13:03:00 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd076f812315c9fe57fc4dcfeb78d3ca2730c9c7e981de075a3776d1a1fa70c1`  
		Last Modified: Thu, 17 Dec 2020 13:03:05 GMT  
		Size: 43.7 MB (43690234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c678945eb0c6c5db1a682aeaa196379e7fb6d0595cfd894705d461e491a46233`  
		Last Modified: Thu, 17 Dec 2020 13:02:58 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3d69439ccb87708f1130cc37520f190c34b9969a84d94e9012487e79a9f5fa`  
		Last Modified: Thu, 17 Dec 2020 13:03:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12aebad2acc6d1f1636a68991f1393c5930c551b34aa6efcc8a30865e9f7c335`  
		Last Modified: Thu, 17 Dec 2020 13:02:59 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm variant v6

```console
$ docker pull consul@sha256:60ccc89b66b6d6b919bfdd1a9c97e0b2beceeeba7fa32213c9c6808f290568db
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41751811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:739a753830be60804b959e2967a22273fcfe6bc193dbf8084e5b336051941ca5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:15:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 17 Dec 2020 01:16:17 GMT
ENV CONSUL_VERSION=1.8.7
# Thu, 17 Dec 2020 01:16:19 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Dec 2020 01:16:22 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Dec 2020 01:16:31 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Dec 2020 01:16:34 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Dec 2020 01:16:39 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:16:43 GMT
VOLUME [/consul/data]
# Thu, 17 Dec 2020 01:16:45 GMT
EXPOSE 8300
# Thu, 17 Dec 2020 01:16:48 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Dec 2020 01:16:49 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Dec 2020 01:16:50 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Dec 2020 01:16:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:16:52 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba9f42fe3e2ae98eae5d07944dddbc958c92651476f2d27e1b0e5cee08ab699`  
		Last Modified: Thu, 17 Dec 2020 01:18:16 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8190afa8d922787587d04afa8bacd88d11e682e306c328dd57ab7493e7bf7757`  
		Last Modified: Thu, 17 Dec 2020 01:18:31 GMT  
		Size: 39.1 MB (39144354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86faa45d46313838e6c819c9e82852f8eb94694588cf7fd48af8caaa85567fe`  
		Last Modified: Thu, 17 Dec 2020 01:18:16 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8db1f794b6327c21e8244715988cb4a7ec8b9fc363df1b0a83b2c735946808`  
		Last Modified: Thu, 17 Dec 2020 01:18:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7dd21bfb8732b48849cf18052a859db85836eceae8a87bcb573b484e240c93`  
		Last Modified: Thu, 17 Dec 2020 01:18:18 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:2b4940197cec37b67509cde36fcca603ac25aea820b9b43eebec924629e95c9a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41924844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac02f425df46003e12ee4a43a76a7c6452f65aafc4ce6b824ab5182e632077c2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:36:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 17 Dec 2020 00:37:15 GMT
ENV CONSUL_VERSION=1.8.7
# Thu, 17 Dec 2020 00:37:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Dec 2020 00:37:18 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Dec 2020 00:37:26 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Dec 2020 00:37:28 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Dec 2020 00:37:31 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 00:37:32 GMT
VOLUME [/consul/data]
# Thu, 17 Dec 2020 00:37:32 GMT
EXPOSE 8300
# Thu, 17 Dec 2020 00:37:33 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Dec 2020 00:37:35 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Dec 2020 00:37:36 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Dec 2020 00:37:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 00:37:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b8c8f97ed381a38a9a343d28b5a08cb8e36a630316cd2a76b159afa5496444`  
		Last Modified: Thu, 17 Dec 2020 00:38:48 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8602e63110fde64304897a07d1b7cbee5d6998a9393ff65c7d95e424caceaae4`  
		Last Modified: Thu, 17 Dec 2020 00:38:58 GMT  
		Size: 39.2 MB (39212508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69bdc80252c65d3edf54957ee8ee16fcb673b76e48f242b48a476d604f215f6`  
		Last Modified: Thu, 17 Dec 2020 00:38:48 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320ed337552e27d977d956f59694971095ced30f76c590ae034106070a1e5464`  
		Last Modified: Thu, 17 Dec 2020 00:38:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2adf14884149b77ee60fd04a7cc9aab126c8fcc9fc1c7716f28ae09799d041f3`  
		Last Modified: Thu, 17 Dec 2020 00:38:48 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; 386

```console
$ docker pull consul@sha256:818b408bc6849112e12da7f3ea394746c42a119179dddf74128ac61bcfe50b77
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (46010063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02e8a0de752b45b100bdd27915124d94b46565f71bd66780e575d461bab48aa9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:24:05 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 17 Dec 2020 01:24:26 GMT
ENV CONSUL_VERSION=1.8.7
# Thu, 17 Dec 2020 01:24:27 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Dec 2020 01:24:27 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Dec 2020 01:24:33 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Dec 2020 01:24:34 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Dec 2020 01:24:35 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:24:35 GMT
VOLUME [/consul/data]
# Thu, 17 Dec 2020 01:24:35 GMT
EXPOSE 8300
# Thu, 17 Dec 2020 01:24:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Dec 2020 01:24:36 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Dec 2020 01:24:36 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Dec 2020 01:24:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:24:36 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34d44d306c927c927cdb0f41e8e65a0a306d60b57dfcaaac94da3cbace1b7a1`  
		Last Modified: Thu, 17 Dec 2020 01:25:37 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c50a053c4ec99cb619df3736cc0e8922dcfd2343aef6968f5df74018b17cc22`  
		Last Modified: Thu, 17 Dec 2020 01:25:45 GMT  
		Size: 43.2 MB (43212701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3586681c47d419fa06e67739ffee0511632fa86031cdea1c10ae3254a34a4160`  
		Last Modified: Thu, 17 Dec 2020 01:25:39 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59fffde0261a7b51ac8ce6986bacd85073713188bb7bf3dae4348b7d87dd55ed`  
		Last Modified: Thu, 17 Dec 2020 01:25:38 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3e5f7f109438fe12ff67f6d063ab7c61814b7cee7591395cffea53990f3bb6`  
		Last Modified: Thu, 17 Dec 2020 01:25:38 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8.7`

```console
$ docker pull consul@sha256:8530be78726dda04dac948a1a707af92af524a76091f42e7da2a7d90dd7ccd1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8.7` - linux; amd64

```console
$ docker pull consul@sha256:eb610ada2181c939654a24803ed28c6eb12afaa728abbf9c44065d10b65c18a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46492534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:811fe376f2881e483cc66f4faf9391f8193ca4620244580af0deb5e0b8238c70`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:01:24 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 17 Dec 2020 13:01:47 GMT
ENV CONSUL_VERSION=1.8.7
# Thu, 17 Dec 2020 13:01:47 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Dec 2020 13:01:49 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Dec 2020 13:01:57 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Dec 2020 13:01:59 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Dec 2020 13:02:00 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:02:01 GMT
VOLUME [/consul/data]
# Thu, 17 Dec 2020 13:02:01 GMT
EXPOSE 8300
# Thu, 17 Dec 2020 13:02:01 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Dec 2020 13:02:02 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Dec 2020 13:02:02 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Dec 2020 13:02:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:02:03 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbaaa36fc2fbe94736d643e90c21a848a00d3d50f9670cc18c0f4abeca674b2`  
		Last Modified: Thu, 17 Dec 2020 13:03:00 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd076f812315c9fe57fc4dcfeb78d3ca2730c9c7e981de075a3776d1a1fa70c1`  
		Last Modified: Thu, 17 Dec 2020 13:03:05 GMT  
		Size: 43.7 MB (43690234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c678945eb0c6c5db1a682aeaa196379e7fb6d0595cfd894705d461e491a46233`  
		Last Modified: Thu, 17 Dec 2020 13:02:58 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3d69439ccb87708f1130cc37520f190c34b9969a84d94e9012487e79a9f5fa`  
		Last Modified: Thu, 17 Dec 2020 13:03:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12aebad2acc6d1f1636a68991f1393c5930c551b34aa6efcc8a30865e9f7c335`  
		Last Modified: Thu, 17 Dec 2020 13:02:59 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.7` - linux; arm variant v6

```console
$ docker pull consul@sha256:60ccc89b66b6d6b919bfdd1a9c97e0b2beceeeba7fa32213c9c6808f290568db
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41751811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:739a753830be60804b959e2967a22273fcfe6bc193dbf8084e5b336051941ca5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:15:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 17 Dec 2020 01:16:17 GMT
ENV CONSUL_VERSION=1.8.7
# Thu, 17 Dec 2020 01:16:19 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Dec 2020 01:16:22 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Dec 2020 01:16:31 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Dec 2020 01:16:34 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Dec 2020 01:16:39 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:16:43 GMT
VOLUME [/consul/data]
# Thu, 17 Dec 2020 01:16:45 GMT
EXPOSE 8300
# Thu, 17 Dec 2020 01:16:48 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Dec 2020 01:16:49 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Dec 2020 01:16:50 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Dec 2020 01:16:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:16:52 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba9f42fe3e2ae98eae5d07944dddbc958c92651476f2d27e1b0e5cee08ab699`  
		Last Modified: Thu, 17 Dec 2020 01:18:16 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8190afa8d922787587d04afa8bacd88d11e682e306c328dd57ab7493e7bf7757`  
		Last Modified: Thu, 17 Dec 2020 01:18:31 GMT  
		Size: 39.1 MB (39144354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86faa45d46313838e6c819c9e82852f8eb94694588cf7fd48af8caaa85567fe`  
		Last Modified: Thu, 17 Dec 2020 01:18:16 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8db1f794b6327c21e8244715988cb4a7ec8b9fc363df1b0a83b2c735946808`  
		Last Modified: Thu, 17 Dec 2020 01:18:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7dd21bfb8732b48849cf18052a859db85836eceae8a87bcb573b484e240c93`  
		Last Modified: Thu, 17 Dec 2020 01:18:18 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.7` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:2b4940197cec37b67509cde36fcca603ac25aea820b9b43eebec924629e95c9a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41924844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac02f425df46003e12ee4a43a76a7c6452f65aafc4ce6b824ab5182e632077c2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:36:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 17 Dec 2020 00:37:15 GMT
ENV CONSUL_VERSION=1.8.7
# Thu, 17 Dec 2020 00:37:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Dec 2020 00:37:18 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Dec 2020 00:37:26 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Dec 2020 00:37:28 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Dec 2020 00:37:31 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 00:37:32 GMT
VOLUME [/consul/data]
# Thu, 17 Dec 2020 00:37:32 GMT
EXPOSE 8300
# Thu, 17 Dec 2020 00:37:33 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Dec 2020 00:37:35 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Dec 2020 00:37:36 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Dec 2020 00:37:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 00:37:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b8c8f97ed381a38a9a343d28b5a08cb8e36a630316cd2a76b159afa5496444`  
		Last Modified: Thu, 17 Dec 2020 00:38:48 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8602e63110fde64304897a07d1b7cbee5d6998a9393ff65c7d95e424caceaae4`  
		Last Modified: Thu, 17 Dec 2020 00:38:58 GMT  
		Size: 39.2 MB (39212508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69bdc80252c65d3edf54957ee8ee16fcb673b76e48f242b48a476d604f215f6`  
		Last Modified: Thu, 17 Dec 2020 00:38:48 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320ed337552e27d977d956f59694971095ced30f76c590ae034106070a1e5464`  
		Last Modified: Thu, 17 Dec 2020 00:38:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2adf14884149b77ee60fd04a7cc9aab126c8fcc9fc1c7716f28ae09799d041f3`  
		Last Modified: Thu, 17 Dec 2020 00:38:48 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.7` - linux; 386

```console
$ docker pull consul@sha256:818b408bc6849112e12da7f3ea394746c42a119179dddf74128ac61bcfe50b77
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (46010063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02e8a0de752b45b100bdd27915124d94b46565f71bd66780e575d461bab48aa9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:24:05 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 17 Dec 2020 01:24:26 GMT
ENV CONSUL_VERSION=1.8.7
# Thu, 17 Dec 2020 01:24:27 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Dec 2020 01:24:27 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Dec 2020 01:24:33 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Dec 2020 01:24:34 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Dec 2020 01:24:35 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:24:35 GMT
VOLUME [/consul/data]
# Thu, 17 Dec 2020 01:24:35 GMT
EXPOSE 8300
# Thu, 17 Dec 2020 01:24:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Dec 2020 01:24:36 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Dec 2020 01:24:36 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Dec 2020 01:24:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:24:36 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34d44d306c927c927cdb0f41e8e65a0a306d60b57dfcaaac94da3cbace1b7a1`  
		Last Modified: Thu, 17 Dec 2020 01:25:37 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c50a053c4ec99cb619df3736cc0e8922dcfd2343aef6968f5df74018b17cc22`  
		Last Modified: Thu, 17 Dec 2020 01:25:45 GMT  
		Size: 43.2 MB (43212701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3586681c47d419fa06e67739ffee0511632fa86031cdea1c10ae3254a34a4160`  
		Last Modified: Thu, 17 Dec 2020 01:25:39 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59fffde0261a7b51ac8ce6986bacd85073713188bb7bf3dae4348b7d87dd55ed`  
		Last Modified: Thu, 17 Dec 2020 01:25:38 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3e5f7f109438fe12ff67f6d063ab7c61814b7cee7591395cffea53990f3bb6`  
		Last Modified: Thu, 17 Dec 2020 01:25:38 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9`

```console
$ docker pull consul@sha256:ee446bdd2e35a9cac8fcfe77fff7dc6f97045eb0cafb8eb283dce7832fc8a45e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9` - linux; amd64

```console
$ docker pull consul@sha256:6f2b6f616ba2c208159379693ed998fed315dc8994c0bf39ee5a29cd2c7b51e0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45572498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2823bc69f80fe3c71d5fd94f188752b28066d118732da47cea866c693a8fe74d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:01:24 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 17 Dec 2020 13:01:25 GMT
ENV CONSUL_VERSION=1.9.1
# Thu, 17 Dec 2020 13:01:25 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Dec 2020 13:01:27 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Dec 2020 13:01:34 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Dec 2020 13:01:35 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Dec 2020 13:01:37 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:01:37 GMT
VOLUME [/consul/data]
# Thu, 17 Dec 2020 13:01:37 GMT
EXPOSE 8300
# Thu, 17 Dec 2020 13:01:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Dec 2020 13:01:38 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Dec 2020 13:01:39 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Dec 2020 13:01:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:01:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365f82ba126180eddf3edbe8597b07845b62ee977e466199c841a7cf6307e6e0`  
		Last Modified: Thu, 17 Dec 2020 13:02:42 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4e74a5b5f7c36a408c2d9a3aca0bdac954e961d7fd85e7be48da3d257192d4`  
		Last Modified: Thu, 17 Dec 2020 13:02:49 GMT  
		Size: 42.8 MB (42770199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ef039d7e5d2b79db3587f87e6d789496e5969106bc837b74c97bb9b1bfd803`  
		Last Modified: Thu, 17 Dec 2020 13:02:41 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a29f03702b28af76b938efacb1f254f9e131c776d0e45dbe6d5616e124f147`  
		Last Modified: Thu, 17 Dec 2020 13:02:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0cc116ba6cdddf467ed810fe5e4047a09cfbf67a763df5aa3e624d23a21ca05`  
		Last Modified: Thu, 17 Dec 2020 13:02:41 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm variant v6

```console
$ docker pull consul@sha256:ced5ef31df69c9d74c2cbacfee3ebb8dcde55e31165083eb72ed3e53ed3b61d3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40834727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5561deb208b18e31f69d3ff33277c300c5cfe66a395bf263d6f8cbda9d2ee260`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:15:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 17 Dec 2020 01:15:30 GMT
ENV CONSUL_VERSION=1.9.1
# Thu, 17 Dec 2020 01:15:31 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Dec 2020 01:15:34 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Dec 2020 01:15:45 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Dec 2020 01:15:50 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Dec 2020 01:15:54 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:15:55 GMT
VOLUME [/consul/data]
# Thu, 17 Dec 2020 01:15:56 GMT
EXPOSE 8300
# Thu, 17 Dec 2020 01:15:58 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Dec 2020 01:16:00 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Dec 2020 01:16:02 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Dec 2020 01:16:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:16:06 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7580055b069041c92f4eb5522a0563cf29e3aa551356fdd3b7b72487b3920bbd`  
		Last Modified: Thu, 17 Dec 2020 01:17:53 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a399fc74cda629e43a8435486fd0bf126ca8344ecbe359c62c15f499093831`  
		Last Modified: Thu, 17 Dec 2020 01:18:05 GMT  
		Size: 38.2 MB (38227270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0afaabff5fcee4e789c167fbeaae2ac1fc1276f93f1251ee20669cb90dfcb3d`  
		Last Modified: Thu, 17 Dec 2020 01:17:52 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4399864fe1d6a07252553f6bb94bd30a2e61ea2afac64312cb869f369b81f017`  
		Last Modified: Thu, 17 Dec 2020 01:17:53 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b17c0404d58db61d873e3b8dc6ebebe59feb7f91b0132b4d5faf9d3883e00cd`  
		Last Modified: Thu, 17 Dec 2020 01:17:52 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:7b878010be55876f2dd419e0e95aad54cd87ae078d5de54e232e4135eb1069c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41054728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2c2dd1235f58df53d892cd4409a01d2296d79bc0659075097fb3e59b5333e5a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:36:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 17 Dec 2020 00:36:46 GMT
ENV CONSUL_VERSION=1.9.1
# Thu, 17 Dec 2020 00:36:47 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Dec 2020 00:36:50 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Dec 2020 00:36:58 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Dec 2020 00:37:01 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Dec 2020 00:37:03 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 00:37:04 GMT
VOLUME [/consul/data]
# Thu, 17 Dec 2020 00:37:05 GMT
EXPOSE 8300
# Thu, 17 Dec 2020 00:37:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Dec 2020 00:37:06 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Dec 2020 00:37:07 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Dec 2020 00:37:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 00:37:09 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24525bced0a98ca04a6bf6cb635d7ace15e937a5e07dd76ea668c8b17a04eef0`  
		Last Modified: Thu, 17 Dec 2020 00:38:29 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e054bc9eeb5c27e7bad342cd91e18906bae54f1a547575e127a457dd16db0822`  
		Last Modified: Thu, 17 Dec 2020 00:38:38 GMT  
		Size: 38.3 MB (38342392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd86a9d50d9ca247d25fde48735e28e11f324632bf1d5dde3a4931999371c99`  
		Last Modified: Thu, 17 Dec 2020 00:38:29 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c07c99456488116d12e65a590c7b4d913b4d439f37335597add07d9d55330b6`  
		Last Modified: Thu, 17 Dec 2020 00:38:29 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1e94d05b445e0a2626bc88419fc01eeaa7e31f09719e972624fb8409a536b2`  
		Last Modified: Thu, 17 Dec 2020 00:38:29 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; 386

```console
$ docker pull consul@sha256:4284d75590380ce58a8023acbb14e7546cd3942af86107e9e2cbb0c93dbba051
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44906113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0d2745507a476ffe17334220110a29eddf92dcdaddaf862b45ddb7aa57d65e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:24:05 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 17 Dec 2020 01:24:05 GMT
ENV CONSUL_VERSION=1.9.1
# Thu, 17 Dec 2020 01:24:06 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Dec 2020 01:24:08 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Dec 2020 01:24:15 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Dec 2020 01:24:16 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Dec 2020 01:24:18 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:24:18 GMT
VOLUME [/consul/data]
# Thu, 17 Dec 2020 01:24:19 GMT
EXPOSE 8300
# Thu, 17 Dec 2020 01:24:19 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Dec 2020 01:24:19 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Dec 2020 01:24:20 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Dec 2020 01:24:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:24:21 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5db229948ed4f23c5fa2a001626e9894183d373f65ac8caaf8d0737f2d9033`  
		Last Modified: Thu, 17 Dec 2020 01:25:16 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c8410709bb1642c76a0f1c8fa9f0f309c9e173662a87301e2f3df4732d9ee3`  
		Last Modified: Thu, 17 Dec 2020 01:25:27 GMT  
		Size: 42.1 MB (42108752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb354e7ccbca6b3933d05091a9ca0d1ba33ceb1555043143ee59628c872b664`  
		Last Modified: Thu, 17 Dec 2020 01:25:16 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95a4e3e62f6116e137fc176d2281871d2181f52caf1cd484c99b37054e614e9e`  
		Last Modified: Thu, 17 Dec 2020 01:25:16 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0e10dadd218a28f522c0276020dab975fbc50ae6ca58763e9246ada1a60c41`  
		Last Modified: Thu, 17 Dec 2020 01:25:16 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9.2`

**does not exist** (yet?)

## `consul:latest`

```console
$ docker pull consul@sha256:ee446bdd2e35a9cac8fcfe77fff7dc6f97045eb0cafb8eb283dce7832fc8a45e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:6f2b6f616ba2c208159379693ed998fed315dc8994c0bf39ee5a29cd2c7b51e0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45572498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2823bc69f80fe3c71d5fd94f188752b28066d118732da47cea866c693a8fe74d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:01:24 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 17 Dec 2020 13:01:25 GMT
ENV CONSUL_VERSION=1.9.1
# Thu, 17 Dec 2020 13:01:25 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Dec 2020 13:01:27 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Dec 2020 13:01:34 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Dec 2020 13:01:35 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Dec 2020 13:01:37 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:01:37 GMT
VOLUME [/consul/data]
# Thu, 17 Dec 2020 13:01:37 GMT
EXPOSE 8300
# Thu, 17 Dec 2020 13:01:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Dec 2020 13:01:38 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Dec 2020 13:01:39 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Dec 2020 13:01:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:01:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365f82ba126180eddf3edbe8597b07845b62ee977e466199c841a7cf6307e6e0`  
		Last Modified: Thu, 17 Dec 2020 13:02:42 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4e74a5b5f7c36a408c2d9a3aca0bdac954e961d7fd85e7be48da3d257192d4`  
		Last Modified: Thu, 17 Dec 2020 13:02:49 GMT  
		Size: 42.8 MB (42770199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ef039d7e5d2b79db3587f87e6d789496e5969106bc837b74c97bb9b1bfd803`  
		Last Modified: Thu, 17 Dec 2020 13:02:41 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a29f03702b28af76b938efacb1f254f9e131c776d0e45dbe6d5616e124f147`  
		Last Modified: Thu, 17 Dec 2020 13:02:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0cc116ba6cdddf467ed810fe5e4047a09cfbf67a763df5aa3e624d23a21ca05`  
		Last Modified: Thu, 17 Dec 2020 13:02:41 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:ced5ef31df69c9d74c2cbacfee3ebb8dcde55e31165083eb72ed3e53ed3b61d3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40834727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5561deb208b18e31f69d3ff33277c300c5cfe66a395bf263d6f8cbda9d2ee260`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:15:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 17 Dec 2020 01:15:30 GMT
ENV CONSUL_VERSION=1.9.1
# Thu, 17 Dec 2020 01:15:31 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Dec 2020 01:15:34 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Dec 2020 01:15:45 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Dec 2020 01:15:50 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Dec 2020 01:15:54 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:15:55 GMT
VOLUME [/consul/data]
# Thu, 17 Dec 2020 01:15:56 GMT
EXPOSE 8300
# Thu, 17 Dec 2020 01:15:58 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Dec 2020 01:16:00 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Dec 2020 01:16:02 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Dec 2020 01:16:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:16:06 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7580055b069041c92f4eb5522a0563cf29e3aa551356fdd3b7b72487b3920bbd`  
		Last Modified: Thu, 17 Dec 2020 01:17:53 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a399fc74cda629e43a8435486fd0bf126ca8344ecbe359c62c15f499093831`  
		Last Modified: Thu, 17 Dec 2020 01:18:05 GMT  
		Size: 38.2 MB (38227270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0afaabff5fcee4e789c167fbeaae2ac1fc1276f93f1251ee20669cb90dfcb3d`  
		Last Modified: Thu, 17 Dec 2020 01:17:52 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4399864fe1d6a07252553f6bb94bd30a2e61ea2afac64312cb869f369b81f017`  
		Last Modified: Thu, 17 Dec 2020 01:17:53 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b17c0404d58db61d873e3b8dc6ebebe59feb7f91b0132b4d5faf9d3883e00cd`  
		Last Modified: Thu, 17 Dec 2020 01:17:52 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:7b878010be55876f2dd419e0e95aad54cd87ae078d5de54e232e4135eb1069c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41054728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2c2dd1235f58df53d892cd4409a01d2296d79bc0659075097fb3e59b5333e5a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:36:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 17 Dec 2020 00:36:46 GMT
ENV CONSUL_VERSION=1.9.1
# Thu, 17 Dec 2020 00:36:47 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Dec 2020 00:36:50 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Dec 2020 00:36:58 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Dec 2020 00:37:01 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Dec 2020 00:37:03 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 00:37:04 GMT
VOLUME [/consul/data]
# Thu, 17 Dec 2020 00:37:05 GMT
EXPOSE 8300
# Thu, 17 Dec 2020 00:37:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Dec 2020 00:37:06 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Dec 2020 00:37:07 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Dec 2020 00:37:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 00:37:09 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24525bced0a98ca04a6bf6cb635d7ace15e937a5e07dd76ea668c8b17a04eef0`  
		Last Modified: Thu, 17 Dec 2020 00:38:29 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e054bc9eeb5c27e7bad342cd91e18906bae54f1a547575e127a457dd16db0822`  
		Last Modified: Thu, 17 Dec 2020 00:38:38 GMT  
		Size: 38.3 MB (38342392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd86a9d50d9ca247d25fde48735e28e11f324632bf1d5dde3a4931999371c99`  
		Last Modified: Thu, 17 Dec 2020 00:38:29 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c07c99456488116d12e65a590c7b4d913b4d439f37335597add07d9d55330b6`  
		Last Modified: Thu, 17 Dec 2020 00:38:29 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1e94d05b445e0a2626bc88419fc01eeaa7e31f09719e972624fb8409a536b2`  
		Last Modified: Thu, 17 Dec 2020 00:38:29 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:4284d75590380ce58a8023acbb14e7546cd3942af86107e9e2cbb0c93dbba051
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44906113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0d2745507a476ffe17334220110a29eddf92dcdaddaf862b45ddb7aa57d65e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:24:05 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 17 Dec 2020 01:24:05 GMT
ENV CONSUL_VERSION=1.9.1
# Thu, 17 Dec 2020 01:24:06 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Dec 2020 01:24:08 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Dec 2020 01:24:15 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Dec 2020 01:24:16 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Dec 2020 01:24:18 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:24:18 GMT
VOLUME [/consul/data]
# Thu, 17 Dec 2020 01:24:19 GMT
EXPOSE 8300
# Thu, 17 Dec 2020 01:24:19 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Dec 2020 01:24:19 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Dec 2020 01:24:20 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Dec 2020 01:24:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:24:21 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5db229948ed4f23c5fa2a001626e9894183d373f65ac8caaf8d0737f2d9033`  
		Last Modified: Thu, 17 Dec 2020 01:25:16 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c8410709bb1642c76a0f1c8fa9f0f309c9e173662a87301e2f3df4732d9ee3`  
		Last Modified: Thu, 17 Dec 2020 01:25:27 GMT  
		Size: 42.1 MB (42108752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb354e7ccbca6b3933d05091a9ca0d1ba33ceb1555043143ee59628c872b664`  
		Last Modified: Thu, 17 Dec 2020 01:25:16 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95a4e3e62f6116e137fc176d2281871d2181f52caf1cd484c99b37054e614e9e`  
		Last Modified: Thu, 17 Dec 2020 01:25:16 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0e10dadd218a28f522c0276020dab975fbc50ae6ca58763e9246ada1a60c41`  
		Last Modified: Thu, 17 Dec 2020 01:25:16 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
