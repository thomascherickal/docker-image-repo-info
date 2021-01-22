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
$ docker pull consul@sha256:3b5c20f1ee6cb29741ec390cc4b3e50e02de0ead14b6ada5b1aa8461beb8e29a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9` - linux; amd64

```console
$ docker pull consul@sha256:ef46003c8ca3069848803aafbc803b1a8ffcdcb97034cb34b5f4c4254b2505ff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45598321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70e1bcefc0b32c32a7ece6d078449b12f9c54bd7c1347200df223210bd62405c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:01:24 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 22 Jan 2021 00:33:50 GMT
ARG CONSUL_VERSION=1.9.2
# Fri, 22 Jan 2021 00:33:51 GMT
LABEL org.opencontainers.image.version=1.9.2
# Fri, 22 Jan 2021 00:33:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 22 Jan 2021 00:33:52 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 22 Jan 2021 00:33:57 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 22 Jan 2021 00:33:58 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 22 Jan 2021 00:33:59 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 22 Jan 2021 00:33:59 GMT
VOLUME [/consul/data]
# Fri, 22 Jan 2021 00:33:59 GMT
EXPOSE 8300
# Fri, 22 Jan 2021 00:33:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 22 Jan 2021 00:33:59 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 22 Jan 2021 00:34:00 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 22 Jan 2021 00:34:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Jan 2021 00:34:00 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622eed43c213ca04b014ca29d4bd443d339b4ce1697945724870f3f3be81c18b`  
		Last Modified: Fri, 22 Jan 2021 00:34:24 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063beacf31e763c209cc2be56ab26891df2de15419c483ccd90f4b1d81e0665c`  
		Last Modified: Fri, 22 Jan 2021 00:34:30 GMT  
		Size: 42.8 MB (42796017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2fca495ba473b83faec23d60822f22d3f2a08ced7024784cd9ef938c2d93b5`  
		Last Modified: Fri, 22 Jan 2021 00:34:24 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed07e71d77a7a297e5cf3bf86ef8e802e9e730e1ffbbee7b9c5d7d93e5936284`  
		Last Modified: Fri, 22 Jan 2021 00:34:24 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e475fda5e48743650615e434915ecbfb2e215386499fd5936f757b762b1a8299`  
		Last Modified: Fri, 22 Jan 2021 00:34:24 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm variant v6

```console
$ docker pull consul@sha256:09433ed5adc26846cadd9d07b88b6ca6995452488be29937b4018e00d07b3a2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40846565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a259b57b45460fbaaae246878625657976c75a381d0dbbf8dcca5e5595a3024f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:15:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 21 Jan 2021 21:52:56 GMT
ARG CONSUL_VERSION=1.9.2
# Thu, 21 Jan 2021 21:52:57 GMT
LABEL org.opencontainers.image.version=1.9.2
# Thu, 21 Jan 2021 21:52:58 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 21 Jan 2021 21:53:01 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 21 Jan 2021 21:55:13 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 21 Jan 2021 21:55:18 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 21 Jan 2021 21:55:21 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 21 Jan 2021 21:55:22 GMT
VOLUME [/consul/data]
# Thu, 21 Jan 2021 21:55:23 GMT
EXPOSE 8300
# Thu, 21 Jan 2021 21:55:24 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 21 Jan 2021 21:55:24 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 21 Jan 2021 21:55:25 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 21 Jan 2021 21:55:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 21:55:26 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68886bcad55540156824b7334ba6968f2e2aef5edbbdb7c99ce6778a138e5346`  
		Last Modified: Thu, 21 Jan 2021 21:56:08 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5537d2ff2a79a77ac5c53d677805c1fb4688881a633541faac2a3c4591000b`  
		Last Modified: Thu, 21 Jan 2021 21:56:19 GMT  
		Size: 38.2 MB (38239103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38219ace88131be232012db73dfa3543d0cb585db03a36434b3bedec8de7e2f`  
		Last Modified: Thu, 21 Jan 2021 21:56:08 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02356861ba79b91256c9d428795d7d6aae4f95f07bb09cde3a5ba9a743bf390`  
		Last Modified: Thu, 21 Jan 2021 21:56:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c65106acd946ef239362e33bcabf1b5d9e6adce96283311e72c2f1a928c0f33`  
		Last Modified: Thu, 21 Jan 2021 21:56:09 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:15a1f0753281fde2cb63a501ba190a53aa2fcf9a90db0f0976bc4c9368cfbd35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41065234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac31a930562e08820ffa23c05e3d66c84579594d7cda5eea1107bb6dbc84ca16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:36:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 22 Jan 2021 01:15:22 GMT
ARG CONSUL_VERSION=1.9.2
# Fri, 22 Jan 2021 01:15:22 GMT
LABEL org.opencontainers.image.version=1.9.2
# Fri, 22 Jan 2021 01:15:23 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 22 Jan 2021 01:15:25 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 22 Jan 2021 01:15:32 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 22 Jan 2021 01:15:34 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 22 Jan 2021 01:15:36 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 22 Jan 2021 01:15:37 GMT
VOLUME [/consul/data]
# Fri, 22 Jan 2021 01:15:37 GMT
EXPOSE 8300
# Fri, 22 Jan 2021 01:15:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 22 Jan 2021 01:15:39 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 22 Jan 2021 01:15:40 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 22 Jan 2021 01:15:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Jan 2021 01:15:41 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bada9d8146f78d35ba9058649f1a743f8f8effe6da47ad7f3efdc994ba55bf41`  
		Last Modified: Fri, 22 Jan 2021 01:16:11 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305af6dcc21c7e5f99fe3059c3f621802851d0a1293fd8c14740b20bb5b75366`  
		Last Modified: Fri, 22 Jan 2021 01:16:19 GMT  
		Size: 38.4 MB (38352892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57dabffb835fa239e023fa6571b5b645ff51b1d40439107a11604e828e316016`  
		Last Modified: Fri, 22 Jan 2021 01:16:10 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd7d264e592997cfd404dd063958d86c708c1ce911ffcfcdd34bbb6ec0e5e79`  
		Last Modified: Fri, 22 Jan 2021 01:16:11 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81738446441aadb1fd34a5df891bf9aca96ae3f40a41bbe34347cae246f212e6`  
		Last Modified: Fri, 22 Jan 2021 01:16:10 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; 386

```console
$ docker pull consul@sha256:bbf964de59b46d6aa23a0f0abfeacf8d92d66ce0974edf11fa883fd93d5bd05b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44918842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97373824e761cbabe5bb17cedd6494eebab31799e05d0cbea58aba0fe1b5a053`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:24:05 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 22 Jan 2021 00:00:45 GMT
ARG CONSUL_VERSION=1.9.2
# Fri, 22 Jan 2021 00:00:45 GMT
LABEL org.opencontainers.image.version=1.9.2
# Fri, 22 Jan 2021 00:00:45 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 22 Jan 2021 00:00:46 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 22 Jan 2021 00:00:58 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 22 Jan 2021 00:00:59 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 22 Jan 2021 00:00:59 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 22 Jan 2021 00:01:00 GMT
VOLUME [/consul/data]
# Fri, 22 Jan 2021 00:01:00 GMT
EXPOSE 8300
# Fri, 22 Jan 2021 00:01:00 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 22 Jan 2021 00:01:00 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 22 Jan 2021 00:01:01 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 22 Jan 2021 00:01:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Jan 2021 00:01:01 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a28b498a655e5f63890364a4aa4a6fa70282b3986dd0b8034ff978a8df9aebf`  
		Last Modified: Fri, 22 Jan 2021 00:01:26 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc789b9b6618677a18b9813121f06f9537a1daf5ff84893bedf1a309edf4b96`  
		Last Modified: Fri, 22 Jan 2021 00:01:37 GMT  
		Size: 42.1 MB (42121475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d93e16ee5f3a25d893087303645ad2d1921100f838b7de5176e4ca260ae6ccc`  
		Last Modified: Fri, 22 Jan 2021 00:01:28 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291d8059ab881bb3fede51f0f18655ab4d0957d84c57d6b69d51d69582ab4c8e`  
		Last Modified: Fri, 22 Jan 2021 00:01:26 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afdaec594273374dd2b6213921b5234defa2b8a3945b484db4e6863f2167968`  
		Last Modified: Fri, 22 Jan 2021 00:01:26 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9.2`

```console
$ docker pull consul@sha256:3b5c20f1ee6cb29741ec390cc4b3e50e02de0ead14b6ada5b1aa8461beb8e29a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9.2` - linux; amd64

```console
$ docker pull consul@sha256:ef46003c8ca3069848803aafbc803b1a8ffcdcb97034cb34b5f4c4254b2505ff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45598321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70e1bcefc0b32c32a7ece6d078449b12f9c54bd7c1347200df223210bd62405c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:01:24 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 22 Jan 2021 00:33:50 GMT
ARG CONSUL_VERSION=1.9.2
# Fri, 22 Jan 2021 00:33:51 GMT
LABEL org.opencontainers.image.version=1.9.2
# Fri, 22 Jan 2021 00:33:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 22 Jan 2021 00:33:52 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 22 Jan 2021 00:33:57 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 22 Jan 2021 00:33:58 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 22 Jan 2021 00:33:59 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 22 Jan 2021 00:33:59 GMT
VOLUME [/consul/data]
# Fri, 22 Jan 2021 00:33:59 GMT
EXPOSE 8300
# Fri, 22 Jan 2021 00:33:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 22 Jan 2021 00:33:59 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 22 Jan 2021 00:34:00 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 22 Jan 2021 00:34:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Jan 2021 00:34:00 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622eed43c213ca04b014ca29d4bd443d339b4ce1697945724870f3f3be81c18b`  
		Last Modified: Fri, 22 Jan 2021 00:34:24 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063beacf31e763c209cc2be56ab26891df2de15419c483ccd90f4b1d81e0665c`  
		Last Modified: Fri, 22 Jan 2021 00:34:30 GMT  
		Size: 42.8 MB (42796017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2fca495ba473b83faec23d60822f22d3f2a08ced7024784cd9ef938c2d93b5`  
		Last Modified: Fri, 22 Jan 2021 00:34:24 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed07e71d77a7a297e5cf3bf86ef8e802e9e730e1ffbbee7b9c5d7d93e5936284`  
		Last Modified: Fri, 22 Jan 2021 00:34:24 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e475fda5e48743650615e434915ecbfb2e215386499fd5936f757b762b1a8299`  
		Last Modified: Fri, 22 Jan 2021 00:34:24 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.2` - linux; arm variant v6

```console
$ docker pull consul@sha256:09433ed5adc26846cadd9d07b88b6ca6995452488be29937b4018e00d07b3a2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40846565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a259b57b45460fbaaae246878625657976c75a381d0dbbf8dcca5e5595a3024f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:15:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 21 Jan 2021 21:52:56 GMT
ARG CONSUL_VERSION=1.9.2
# Thu, 21 Jan 2021 21:52:57 GMT
LABEL org.opencontainers.image.version=1.9.2
# Thu, 21 Jan 2021 21:52:58 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 21 Jan 2021 21:53:01 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 21 Jan 2021 21:55:13 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 21 Jan 2021 21:55:18 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 21 Jan 2021 21:55:21 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 21 Jan 2021 21:55:22 GMT
VOLUME [/consul/data]
# Thu, 21 Jan 2021 21:55:23 GMT
EXPOSE 8300
# Thu, 21 Jan 2021 21:55:24 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 21 Jan 2021 21:55:24 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 21 Jan 2021 21:55:25 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 21 Jan 2021 21:55:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 21:55:26 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68886bcad55540156824b7334ba6968f2e2aef5edbbdb7c99ce6778a138e5346`  
		Last Modified: Thu, 21 Jan 2021 21:56:08 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5537d2ff2a79a77ac5c53d677805c1fb4688881a633541faac2a3c4591000b`  
		Last Modified: Thu, 21 Jan 2021 21:56:19 GMT  
		Size: 38.2 MB (38239103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38219ace88131be232012db73dfa3543d0cb585db03a36434b3bedec8de7e2f`  
		Last Modified: Thu, 21 Jan 2021 21:56:08 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02356861ba79b91256c9d428795d7d6aae4f95f07bb09cde3a5ba9a743bf390`  
		Last Modified: Thu, 21 Jan 2021 21:56:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c65106acd946ef239362e33bcabf1b5d9e6adce96283311e72c2f1a928c0f33`  
		Last Modified: Thu, 21 Jan 2021 21:56:09 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.2` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:15a1f0753281fde2cb63a501ba190a53aa2fcf9a90db0f0976bc4c9368cfbd35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41065234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac31a930562e08820ffa23c05e3d66c84579594d7cda5eea1107bb6dbc84ca16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:36:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 22 Jan 2021 01:15:22 GMT
ARG CONSUL_VERSION=1.9.2
# Fri, 22 Jan 2021 01:15:22 GMT
LABEL org.opencontainers.image.version=1.9.2
# Fri, 22 Jan 2021 01:15:23 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 22 Jan 2021 01:15:25 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 22 Jan 2021 01:15:32 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 22 Jan 2021 01:15:34 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 22 Jan 2021 01:15:36 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 22 Jan 2021 01:15:37 GMT
VOLUME [/consul/data]
# Fri, 22 Jan 2021 01:15:37 GMT
EXPOSE 8300
# Fri, 22 Jan 2021 01:15:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 22 Jan 2021 01:15:39 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 22 Jan 2021 01:15:40 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 22 Jan 2021 01:15:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Jan 2021 01:15:41 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bada9d8146f78d35ba9058649f1a743f8f8effe6da47ad7f3efdc994ba55bf41`  
		Last Modified: Fri, 22 Jan 2021 01:16:11 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305af6dcc21c7e5f99fe3059c3f621802851d0a1293fd8c14740b20bb5b75366`  
		Last Modified: Fri, 22 Jan 2021 01:16:19 GMT  
		Size: 38.4 MB (38352892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57dabffb835fa239e023fa6571b5b645ff51b1d40439107a11604e828e316016`  
		Last Modified: Fri, 22 Jan 2021 01:16:10 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd7d264e592997cfd404dd063958d86c708c1ce911ffcfcdd34bbb6ec0e5e79`  
		Last Modified: Fri, 22 Jan 2021 01:16:11 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81738446441aadb1fd34a5df891bf9aca96ae3f40a41bbe34347cae246f212e6`  
		Last Modified: Fri, 22 Jan 2021 01:16:10 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.2` - linux; 386

```console
$ docker pull consul@sha256:bbf964de59b46d6aa23a0f0abfeacf8d92d66ce0974edf11fa883fd93d5bd05b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44918842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97373824e761cbabe5bb17cedd6494eebab31799e05d0cbea58aba0fe1b5a053`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:24:05 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 22 Jan 2021 00:00:45 GMT
ARG CONSUL_VERSION=1.9.2
# Fri, 22 Jan 2021 00:00:45 GMT
LABEL org.opencontainers.image.version=1.9.2
# Fri, 22 Jan 2021 00:00:45 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 22 Jan 2021 00:00:46 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 22 Jan 2021 00:00:58 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 22 Jan 2021 00:00:59 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 22 Jan 2021 00:00:59 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 22 Jan 2021 00:01:00 GMT
VOLUME [/consul/data]
# Fri, 22 Jan 2021 00:01:00 GMT
EXPOSE 8300
# Fri, 22 Jan 2021 00:01:00 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 22 Jan 2021 00:01:00 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 22 Jan 2021 00:01:01 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 22 Jan 2021 00:01:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Jan 2021 00:01:01 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a28b498a655e5f63890364a4aa4a6fa70282b3986dd0b8034ff978a8df9aebf`  
		Last Modified: Fri, 22 Jan 2021 00:01:26 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc789b9b6618677a18b9813121f06f9537a1daf5ff84893bedf1a309edf4b96`  
		Last Modified: Fri, 22 Jan 2021 00:01:37 GMT  
		Size: 42.1 MB (42121475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d93e16ee5f3a25d893087303645ad2d1921100f838b7de5176e4ca260ae6ccc`  
		Last Modified: Fri, 22 Jan 2021 00:01:28 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291d8059ab881bb3fede51f0f18655ab4d0957d84c57d6b69d51d69582ab4c8e`  
		Last Modified: Fri, 22 Jan 2021 00:01:26 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afdaec594273374dd2b6213921b5234defa2b8a3945b484db4e6863f2167968`  
		Last Modified: Fri, 22 Jan 2021 00:01:26 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:3b5c20f1ee6cb29741ec390cc4b3e50e02de0ead14b6ada5b1aa8461beb8e29a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:ef46003c8ca3069848803aafbc803b1a8ffcdcb97034cb34b5f4c4254b2505ff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45598321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70e1bcefc0b32c32a7ece6d078449b12f9c54bd7c1347200df223210bd62405c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:01:24 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 22 Jan 2021 00:33:50 GMT
ARG CONSUL_VERSION=1.9.2
# Fri, 22 Jan 2021 00:33:51 GMT
LABEL org.opencontainers.image.version=1.9.2
# Fri, 22 Jan 2021 00:33:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 22 Jan 2021 00:33:52 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 22 Jan 2021 00:33:57 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 22 Jan 2021 00:33:58 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 22 Jan 2021 00:33:59 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 22 Jan 2021 00:33:59 GMT
VOLUME [/consul/data]
# Fri, 22 Jan 2021 00:33:59 GMT
EXPOSE 8300
# Fri, 22 Jan 2021 00:33:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 22 Jan 2021 00:33:59 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 22 Jan 2021 00:34:00 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 22 Jan 2021 00:34:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Jan 2021 00:34:00 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622eed43c213ca04b014ca29d4bd443d339b4ce1697945724870f3f3be81c18b`  
		Last Modified: Fri, 22 Jan 2021 00:34:24 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063beacf31e763c209cc2be56ab26891df2de15419c483ccd90f4b1d81e0665c`  
		Last Modified: Fri, 22 Jan 2021 00:34:30 GMT  
		Size: 42.8 MB (42796017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2fca495ba473b83faec23d60822f22d3f2a08ced7024784cd9ef938c2d93b5`  
		Last Modified: Fri, 22 Jan 2021 00:34:24 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed07e71d77a7a297e5cf3bf86ef8e802e9e730e1ffbbee7b9c5d7d93e5936284`  
		Last Modified: Fri, 22 Jan 2021 00:34:24 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e475fda5e48743650615e434915ecbfb2e215386499fd5936f757b762b1a8299`  
		Last Modified: Fri, 22 Jan 2021 00:34:24 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:09433ed5adc26846cadd9d07b88b6ca6995452488be29937b4018e00d07b3a2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40846565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a259b57b45460fbaaae246878625657976c75a381d0dbbf8dcca5e5595a3024f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:15:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 21 Jan 2021 21:52:56 GMT
ARG CONSUL_VERSION=1.9.2
# Thu, 21 Jan 2021 21:52:57 GMT
LABEL org.opencontainers.image.version=1.9.2
# Thu, 21 Jan 2021 21:52:58 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 21 Jan 2021 21:53:01 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 21 Jan 2021 21:55:13 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 21 Jan 2021 21:55:18 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 21 Jan 2021 21:55:21 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 21 Jan 2021 21:55:22 GMT
VOLUME [/consul/data]
# Thu, 21 Jan 2021 21:55:23 GMT
EXPOSE 8300
# Thu, 21 Jan 2021 21:55:24 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 21 Jan 2021 21:55:24 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 21 Jan 2021 21:55:25 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 21 Jan 2021 21:55:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 21:55:26 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68886bcad55540156824b7334ba6968f2e2aef5edbbdb7c99ce6778a138e5346`  
		Last Modified: Thu, 21 Jan 2021 21:56:08 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5537d2ff2a79a77ac5c53d677805c1fb4688881a633541faac2a3c4591000b`  
		Last Modified: Thu, 21 Jan 2021 21:56:19 GMT  
		Size: 38.2 MB (38239103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38219ace88131be232012db73dfa3543d0cb585db03a36434b3bedec8de7e2f`  
		Last Modified: Thu, 21 Jan 2021 21:56:08 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02356861ba79b91256c9d428795d7d6aae4f95f07bb09cde3a5ba9a743bf390`  
		Last Modified: Thu, 21 Jan 2021 21:56:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c65106acd946ef239362e33bcabf1b5d9e6adce96283311e72c2f1a928c0f33`  
		Last Modified: Thu, 21 Jan 2021 21:56:09 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:15a1f0753281fde2cb63a501ba190a53aa2fcf9a90db0f0976bc4c9368cfbd35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41065234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac31a930562e08820ffa23c05e3d66c84579594d7cda5eea1107bb6dbc84ca16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:36:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 22 Jan 2021 01:15:22 GMT
ARG CONSUL_VERSION=1.9.2
# Fri, 22 Jan 2021 01:15:22 GMT
LABEL org.opencontainers.image.version=1.9.2
# Fri, 22 Jan 2021 01:15:23 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 22 Jan 2021 01:15:25 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 22 Jan 2021 01:15:32 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 22 Jan 2021 01:15:34 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 22 Jan 2021 01:15:36 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 22 Jan 2021 01:15:37 GMT
VOLUME [/consul/data]
# Fri, 22 Jan 2021 01:15:37 GMT
EXPOSE 8300
# Fri, 22 Jan 2021 01:15:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 22 Jan 2021 01:15:39 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 22 Jan 2021 01:15:40 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 22 Jan 2021 01:15:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Jan 2021 01:15:41 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bada9d8146f78d35ba9058649f1a743f8f8effe6da47ad7f3efdc994ba55bf41`  
		Last Modified: Fri, 22 Jan 2021 01:16:11 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305af6dcc21c7e5f99fe3059c3f621802851d0a1293fd8c14740b20bb5b75366`  
		Last Modified: Fri, 22 Jan 2021 01:16:19 GMT  
		Size: 38.4 MB (38352892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57dabffb835fa239e023fa6571b5b645ff51b1d40439107a11604e828e316016`  
		Last Modified: Fri, 22 Jan 2021 01:16:10 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd7d264e592997cfd404dd063958d86c708c1ce911ffcfcdd34bbb6ec0e5e79`  
		Last Modified: Fri, 22 Jan 2021 01:16:11 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81738446441aadb1fd34a5df891bf9aca96ae3f40a41bbe34347cae246f212e6`  
		Last Modified: Fri, 22 Jan 2021 01:16:10 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:bbf964de59b46d6aa23a0f0abfeacf8d92d66ce0974edf11fa883fd93d5bd05b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44918842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97373824e761cbabe5bb17cedd6494eebab31799e05d0cbea58aba0fe1b5a053`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:24:05 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 22 Jan 2021 00:00:45 GMT
ARG CONSUL_VERSION=1.9.2
# Fri, 22 Jan 2021 00:00:45 GMT
LABEL org.opencontainers.image.version=1.9.2
# Fri, 22 Jan 2021 00:00:45 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 22 Jan 2021 00:00:46 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 22 Jan 2021 00:00:58 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 22 Jan 2021 00:00:59 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 22 Jan 2021 00:00:59 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 22 Jan 2021 00:01:00 GMT
VOLUME [/consul/data]
# Fri, 22 Jan 2021 00:01:00 GMT
EXPOSE 8300
# Fri, 22 Jan 2021 00:01:00 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 22 Jan 2021 00:01:00 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 22 Jan 2021 00:01:01 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 22 Jan 2021 00:01:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Jan 2021 00:01:01 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a28b498a655e5f63890364a4aa4a6fa70282b3986dd0b8034ff978a8df9aebf`  
		Last Modified: Fri, 22 Jan 2021 00:01:26 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc789b9b6618677a18b9813121f06f9537a1daf5ff84893bedf1a309edf4b96`  
		Last Modified: Fri, 22 Jan 2021 00:01:37 GMT  
		Size: 42.1 MB (42121475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d93e16ee5f3a25d893087303645ad2d1921100f838b7de5176e4ca260ae6ccc`  
		Last Modified: Fri, 22 Jan 2021 00:01:28 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291d8059ab881bb3fede51f0f18655ab4d0957d84c57d6b69d51d69582ab4c8e`  
		Last Modified: Fri, 22 Jan 2021 00:01:26 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afdaec594273374dd2b6213921b5234defa2b8a3945b484db4e6863f2167968`  
		Last Modified: Fri, 22 Jan 2021 00:01:26 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
