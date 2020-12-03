<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.6`](#consul16)
-	[`consul:1.6.10`](#consul1610)
-	[`consul:1.7`](#consul17)
-	[`consul:1.7.10`](#consul1710)
-	[`consul:1.8`](#consul18)
-	[`consul:1.8.6`](#consul186)
-	[`consul:1.8.7-beta1`](#consul187-beta1)
-	[`consul:1.9`](#consul19)
-	[`consul:1.9.0`](#consul190)
-	[`consul:latest`](#consullatest)

## `consul:1.6`

```console
$ docker pull consul@sha256:d1989d99ca5d1363557af7af6e7f8c88a6fca918d074b1d9b6a00e4d2081eaaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.6` - linux; amd64

```console
$ docker pull consul@sha256:540f9ab6b680ef0652968b89c1e99fc8a5946c22f7aa785bde1eeb4d6a62ca41
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45175636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5458ab179d388608ebf629abe3de94f709a1fb3efe6d7e6d589c0b646bc6e20`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:17:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:20:10 GMT
ENV CONSUL_VERSION=1.6.10
# Sat, 21 Nov 2020 01:20:10 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:20:11 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:20:16 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     apk -X https://dl-cdn.alpinelinux.org/alpine/v3.8/main add tzdata=2020a-r0 &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:20:17 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:20:18 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:20:19 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:20:19 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:20:19 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:20:19 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:20:19 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:20:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:20:20 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5d842dca06679337d51647be9098c4f50478e39ecdf2c273f7041f4f44cb05`  
		Last Modified: Sat, 21 Nov 2020 01:20:58 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4254a7a05e76ce9973454a9d03643f5ff8e3c5ae7546918922822d52cdfe0a`  
		Last Modified: Sat, 21 Nov 2020 01:21:18 GMT  
		Size: 42.4 MB (42375538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add8f1f252a13951ceab6b861d413e350d5493b0ca94b982165543995b1185eb`  
		Last Modified: Sat, 21 Nov 2020 01:20:57 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be248510e3639779501a06f62f9b0d5c31e6f19adebf1737707c881888d5279`  
		Last Modified: Sat, 21 Nov 2020 01:20:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85d455a373ed7d502e81195c86141a42c45bfe4fbfaefbf0024e148feb0560`  
		Last Modified: Sat, 21 Nov 2020 01:20:57 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; arm variant v6

```console
$ docker pull consul@sha256:3d16e27dbd80e122713a7abb4c4ce7976d1ee5faeddc99316825321a71474372
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40611108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36ccd5a279004be4fa388a1bcdf8b8365539a30fd602a40808c19e6ef82ed596`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:17:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:52:01 GMT
ENV CONSUL_VERSION=1.6.10
# Sat, 21 Nov 2020 01:52:02 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:52:03 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:52:13 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     apk -X https://dl-cdn.alpinelinux.org/alpine/v3.8/main add tzdata=2020a-r0 &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:52:15 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:52:16 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:52:17 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:52:18 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:52:18 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:52:19 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:52:19 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:52:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:52:21 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299e8387711c42f9833a0f6a8486c3a9ef2a636f01c2f4e6d2500f65ef497447`  
		Last Modified: Sat, 21 Nov 2020 01:53:14 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba1a8d686c527655780d0b9d1f43030f3c83c6124ece9a4f2a2a9eab8efc254`  
		Last Modified: Sat, 21 Nov 2020 01:53:24 GMT  
		Size: 38.0 MB (38005904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a39f5f1ad9553f69b60b8e6838c3641a964a21ff4782bea731d9bb45cfe93c`  
		Last Modified: Sat, 21 Nov 2020 01:53:14 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e45d38492c8e656be41694bbeca2a3bcd60fbe80646b79e8fed479bbb5a7739`  
		Last Modified: Sat, 21 Nov 2020 01:53:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d52ddce60c01097cae445608b13b8ec019745ebc22b412c61bcae9da6381137`  
		Last Modified: Sat, 21 Nov 2020 01:53:14 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:92061681bb594e70c9f91cf874d27c062445462566a97a64fe345565677006c5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (41048179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:845cddec463dccfcedd8418401c1f042740d2d1778895c0af7f70447f16991bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:42:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:41:06 GMT
ENV CONSUL_VERSION=1.6.10
# Sat, 21 Nov 2020 01:41:07 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:41:09 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:41:17 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     apk -X https://dl-cdn.alpinelinux.org/alpine/v3.8/main add tzdata=2020a-r0 &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:41:20 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:41:21 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:41:22 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:41:23 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:41:24 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:41:25 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:41:26 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:41:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:41:27 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40208d4b1481cbea89e5048238270fe3b31233bdeebbd2976eabba81c4d20f8`  
		Last Modified: Sat, 21 Nov 2020 01:42:16 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e59480e92a014ac01fde03bf2469707d9e8499240b02983a89c8844252c516a`  
		Last Modified: Sat, 21 Nov 2020 01:42:25 GMT  
		Size: 38.3 MB (38338330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492f92778006e76a49f48043533c669db7000681b547857219d882fbb70cdf2a`  
		Last Modified: Sat, 21 Nov 2020 01:42:16 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1427fa4101529169daa91c0e54cf89eec60cff8b9a0641d6f27326908bfad83b`  
		Last Modified: Sat, 21 Nov 2020 01:42:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e5ee59295b508b3ed6f278fa14f5aa99fa7c8e485e2148618abb969b88072a`  
		Last Modified: Sat, 21 Nov 2020 01:42:16 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; 386

```console
$ docker pull consul@sha256:4e0f5cacbf900e90e3aab47c6dd8f07d057a792e7f45aae0236f27d2fbb33ab4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43952807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:044965116ab4acbbd2bf8bfc28c6b639f9481aad24c9de88722e24bbd3b75b35`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:39:11 GMT
ENV CONSUL_VERSION=1.6.10
# Sat, 21 Nov 2020 01:39:11 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:39:12 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:39:19 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     apk -X https://dl-cdn.alpinelinux.org/alpine/v3.8/main add tzdata=2020a-r0 &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:39:19 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:39:20 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:39:20 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:39:21 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:39:21 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:39:21 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:39:21 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:39:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:39:22 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073955cd82a1400897e9e8c0f871d7b3382f2bd068abd5e4523ff14758e2e908`  
		Last Modified: Sat, 21 Nov 2020 01:40:05 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c3020e8d98304dd9177e08ba742685d53a076f9807fd4ef84a1f3109abaf2e`  
		Last Modified: Sat, 21 Nov 2020 01:40:14 GMT  
		Size: 41.2 MB (41158168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e881d4d393cffbf1679126019e5c1dabe5ed7875a78005f7b2570cce62c46ae`  
		Last Modified: Sat, 21 Nov 2020 01:40:04 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819b2209f9062b82406066a16ac9005018f448a0c1bc06f426c031f864b05ebd`  
		Last Modified: Sat, 21 Nov 2020 01:40:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b2426aa309c8071a39df0069984a071114bb3777032933745d60603f0a5fea`  
		Last Modified: Sat, 21 Nov 2020 01:40:05 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.6.10`

```console
$ docker pull consul@sha256:d1989d99ca5d1363557af7af6e7f8c88a6fca918d074b1d9b6a00e4d2081eaaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.6.10` - linux; amd64

```console
$ docker pull consul@sha256:540f9ab6b680ef0652968b89c1e99fc8a5946c22f7aa785bde1eeb4d6a62ca41
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45175636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5458ab179d388608ebf629abe3de94f709a1fb3efe6d7e6d589c0b646bc6e20`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:17:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:20:10 GMT
ENV CONSUL_VERSION=1.6.10
# Sat, 21 Nov 2020 01:20:10 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:20:11 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:20:16 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     apk -X https://dl-cdn.alpinelinux.org/alpine/v3.8/main add tzdata=2020a-r0 &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:20:17 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:20:18 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:20:19 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:20:19 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:20:19 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:20:19 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:20:19 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:20:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:20:20 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5d842dca06679337d51647be9098c4f50478e39ecdf2c273f7041f4f44cb05`  
		Last Modified: Sat, 21 Nov 2020 01:20:58 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4254a7a05e76ce9973454a9d03643f5ff8e3c5ae7546918922822d52cdfe0a`  
		Last Modified: Sat, 21 Nov 2020 01:21:18 GMT  
		Size: 42.4 MB (42375538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add8f1f252a13951ceab6b861d413e350d5493b0ca94b982165543995b1185eb`  
		Last Modified: Sat, 21 Nov 2020 01:20:57 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be248510e3639779501a06f62f9b0d5c31e6f19adebf1737707c881888d5279`  
		Last Modified: Sat, 21 Nov 2020 01:20:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85d455a373ed7d502e81195c86141a42c45bfe4fbfaefbf0024e148feb0560`  
		Last Modified: Sat, 21 Nov 2020 01:20:57 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6.10` - linux; arm variant v6

```console
$ docker pull consul@sha256:3d16e27dbd80e122713a7abb4c4ce7976d1ee5faeddc99316825321a71474372
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40611108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36ccd5a279004be4fa388a1bcdf8b8365539a30fd602a40808c19e6ef82ed596`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:17:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:52:01 GMT
ENV CONSUL_VERSION=1.6.10
# Sat, 21 Nov 2020 01:52:02 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:52:03 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:52:13 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     apk -X https://dl-cdn.alpinelinux.org/alpine/v3.8/main add tzdata=2020a-r0 &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:52:15 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:52:16 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:52:17 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:52:18 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:52:18 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:52:19 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:52:19 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:52:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:52:21 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299e8387711c42f9833a0f6a8486c3a9ef2a636f01c2f4e6d2500f65ef497447`  
		Last Modified: Sat, 21 Nov 2020 01:53:14 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba1a8d686c527655780d0b9d1f43030f3c83c6124ece9a4f2a2a9eab8efc254`  
		Last Modified: Sat, 21 Nov 2020 01:53:24 GMT  
		Size: 38.0 MB (38005904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a39f5f1ad9553f69b60b8e6838c3641a964a21ff4782bea731d9bb45cfe93c`  
		Last Modified: Sat, 21 Nov 2020 01:53:14 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e45d38492c8e656be41694bbeca2a3bcd60fbe80646b79e8fed479bbb5a7739`  
		Last Modified: Sat, 21 Nov 2020 01:53:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d52ddce60c01097cae445608b13b8ec019745ebc22b412c61bcae9da6381137`  
		Last Modified: Sat, 21 Nov 2020 01:53:14 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6.10` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:92061681bb594e70c9f91cf874d27c062445462566a97a64fe345565677006c5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (41048179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:845cddec463dccfcedd8418401c1f042740d2d1778895c0af7f70447f16991bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:42:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:41:06 GMT
ENV CONSUL_VERSION=1.6.10
# Sat, 21 Nov 2020 01:41:07 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:41:09 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:41:17 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     apk -X https://dl-cdn.alpinelinux.org/alpine/v3.8/main add tzdata=2020a-r0 &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:41:20 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:41:21 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:41:22 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:41:23 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:41:24 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:41:25 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:41:26 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:41:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:41:27 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40208d4b1481cbea89e5048238270fe3b31233bdeebbd2976eabba81c4d20f8`  
		Last Modified: Sat, 21 Nov 2020 01:42:16 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e59480e92a014ac01fde03bf2469707d9e8499240b02983a89c8844252c516a`  
		Last Modified: Sat, 21 Nov 2020 01:42:25 GMT  
		Size: 38.3 MB (38338330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492f92778006e76a49f48043533c669db7000681b547857219d882fbb70cdf2a`  
		Last Modified: Sat, 21 Nov 2020 01:42:16 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1427fa4101529169daa91c0e54cf89eec60cff8b9a0641d6f27326908bfad83b`  
		Last Modified: Sat, 21 Nov 2020 01:42:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e5ee59295b508b3ed6f278fa14f5aa99fa7c8e485e2148618abb969b88072a`  
		Last Modified: Sat, 21 Nov 2020 01:42:16 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6.10` - linux; 386

```console
$ docker pull consul@sha256:4e0f5cacbf900e90e3aab47c6dd8f07d057a792e7f45aae0236f27d2fbb33ab4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43952807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:044965116ab4acbbd2bf8bfc28c6b639f9481aad24c9de88722e24bbd3b75b35`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:39:11 GMT
ENV CONSUL_VERSION=1.6.10
# Sat, 21 Nov 2020 01:39:11 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:39:12 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:39:19 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     apk -X https://dl-cdn.alpinelinux.org/alpine/v3.8/main add tzdata=2020a-r0 &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:39:19 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:39:20 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:39:20 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:39:21 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:39:21 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:39:21 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:39:21 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:39:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:39:22 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073955cd82a1400897e9e8c0f871d7b3382f2bd068abd5e4523ff14758e2e908`  
		Last Modified: Sat, 21 Nov 2020 01:40:05 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c3020e8d98304dd9177e08ba742685d53a076f9807fd4ef84a1f3109abaf2e`  
		Last Modified: Sat, 21 Nov 2020 01:40:14 GMT  
		Size: 41.2 MB (41158168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e881d4d393cffbf1679126019e5c1dabe5ed7875a78005f7b2570cce62c46ae`  
		Last Modified: Sat, 21 Nov 2020 01:40:04 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819b2209f9062b82406066a16ac9005018f448a0c1bc06f426c031f864b05ebd`  
		Last Modified: Sat, 21 Nov 2020 01:40:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b2426aa309c8071a39df0069984a071114bb3777032933745d60603f0a5fea`  
		Last Modified: Sat, 21 Nov 2020 01:40:05 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7`

```console
$ docker pull consul@sha256:faf065e1f8f126808433936893e73d2ec29d470639144440c80d863652da8e36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7` - linux; amd64

```console
$ docker pull consul@sha256:550925ee4e2239473e056018a046936792e7a6152f81b90dfac729860319591d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.5 MB (43475728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2430b3580607697c33f4cb88d1cc9cc07d947f0fb5d39c4bd7b317fb309533b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:17:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:19:56 GMT
ENV CONSUL_VERSION=1.7.10
# Sat, 21 Nov 2020 01:19:56 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:19:57 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:20:01 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:20:02 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:20:03 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:20:03 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:20:03 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:20:03 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:20:04 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:20:04 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:20:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:20:04 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca7289d3480a7f27dcc51f696868ab76ca9035d8f944a661bd3e099f1ea78e7`  
		Last Modified: Sat, 21 Nov 2020 01:20:45 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6a7418fece1c5e89caa9a8b68d57bf6b63872ab00bd3859ce7e395553f0407`  
		Last Modified: Sat, 21 Nov 2020 01:20:52 GMT  
		Size: 40.7 MB (40675633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d63f57fc4f6c269ef81dd6fc2a820fdbedd5ab94a5cb506120082ee58054e2`  
		Last Modified: Sat, 21 Nov 2020 01:20:44 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96c54e6fe850cf0048d61bfc9d199e83c415130403528599d7daa7a8540b8b4`  
		Last Modified: Sat, 21 Nov 2020 01:20:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a065ffea4fd3691a75fc16152bada39181b6292a75158a7a75b6d365badc4b60`  
		Last Modified: Sat, 21 Nov 2020 01:20:45 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm variant v6

```console
$ docker pull consul@sha256:9898e52e14bff1b3253c7c2e55f5d96c0b811996d660b95c9bbbe17c3924e5b2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39188612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dd65b663c29d650428766e072216c95f4bd8175f4d84dac1b503cc28b136f26`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:17:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:51:34 GMT
ENV CONSUL_VERSION=1.7.10
# Sat, 21 Nov 2020 01:51:35 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:51:37 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:51:45 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:51:47 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:51:49 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:51:50 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:51:50 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:51:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:51:52 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:51:52 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:51:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:51:53 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1a095f2c01406b324aecee6ea15b9382a7f9d3911742cc95943b482697b9cd`  
		Last Modified: Sat, 21 Nov 2020 01:52:56 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c1d8fd42c534d53d881613da0bb84d8c43286324887e006b1b7546ac962b65`  
		Last Modified: Sat, 21 Nov 2020 01:53:06 GMT  
		Size: 36.6 MB (36583407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9a2173853dd15d974475841118cbd7e2b13753d79b5c5b2594bfbef4214a5f`  
		Last Modified: Sat, 21 Nov 2020 01:52:56 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c92bac46c11832762dc2ff097f7722ebd2214322f1f27e7145ac1b5368c2a2`  
		Last Modified: Sat, 21 Nov 2020 01:52:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99776bd6406ac1737981c6af30b75ae07dc17d3d0ba2486fb5d2400f6fedebe7`  
		Last Modified: Sat, 21 Nov 2020 01:52:56 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:18e46ed1d4d6cbecfca7efbb99a6004d251e53ad1fd3b09ef568c78092aaa232
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.4 MB (39412443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:459b7ea4c4a47d0867cdbb6f9f6345ba9d98569bc13744b5a414d38f17419cff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:42:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:40:35 GMT
ENV CONSUL_VERSION=1.7.10
# Sat, 21 Nov 2020 01:40:37 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:40:40 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:40:47 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:40:50 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:40:52 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:40:52 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:40:53 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:40:54 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:40:54 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:40:55 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:40:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:40:59 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ca11a9c4f0e01c15269e1a922b3e85cace4c6a4e8012fe46d991c3b631543b`  
		Last Modified: Sat, 21 Nov 2020 01:41:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0deadfb700fc32b539eb184f000ab8428f2e3949738e1395648a45ab6b322a2`  
		Last Modified: Sat, 21 Nov 2020 01:42:08 GMT  
		Size: 36.7 MB (36702593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be84067000b0818bb382343e10626a5a994433c7709d998bfd0fd4f72899e175`  
		Last Modified: Sat, 21 Nov 2020 01:41:59 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2515b9e6d5bca0056bbc4fa69d34ec0bf6e33aa2b86357cc377bda959870c449`  
		Last Modified: Sat, 21 Nov 2020 01:41:59 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c666cac88ee672bc0f44329987bf2a1bc19238d7c54b4e2bd428726f9bff8cd0`  
		Last Modified: Sat, 21 Nov 2020 01:41:59 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; 386

```console
$ docker pull consul@sha256:9060331ac68bc5b49ca118d89b3de037f26d930318384931d8ddae9fdac3689a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42273476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5388bbbe3074d5368f55e8be06633a0207adc15d8b1ed956b25f4932e74d47d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:38:55 GMT
ENV CONSUL_VERSION=1.7.10
# Sat, 21 Nov 2020 01:38:55 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:38:56 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:39:03 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:39:04 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:39:05 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:39:05 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:39:05 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:39:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:39:06 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:39:06 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:39:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:39:07 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad9d9e88674a9ee11182151110497f18d229130a39fa8c6afa877d3f68d7211`  
		Last Modified: Sat, 21 Nov 2020 01:39:49 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c3807ca6a52a3d92cceb7f8c1c3ecd3a0e3bebfcf603fc0e1f18ab493350b3`  
		Last Modified: Sat, 21 Nov 2020 01:40:00 GMT  
		Size: 39.5 MB (39478832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f655fb0d3f657436baef11ac6955a8e4d91c3f95bc563042c8e3ee4a83dca2f`  
		Last Modified: Sat, 21 Nov 2020 01:39:49 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8581f6b37196be59e34bc65d25f14344d505b62347fd78de5598bffac35f0c0`  
		Last Modified: Sat, 21 Nov 2020 01:39:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b6f208b77ae07b8b434483ec34c407e10c1b89b132f816cae1a8d498c9fb92`  
		Last Modified: Sat, 21 Nov 2020 01:39:49 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7.10`

```console
$ docker pull consul@sha256:faf065e1f8f126808433936893e73d2ec29d470639144440c80d863652da8e36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7.10` - linux; amd64

```console
$ docker pull consul@sha256:550925ee4e2239473e056018a046936792e7a6152f81b90dfac729860319591d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.5 MB (43475728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2430b3580607697c33f4cb88d1cc9cc07d947f0fb5d39c4bd7b317fb309533b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:17:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:19:56 GMT
ENV CONSUL_VERSION=1.7.10
# Sat, 21 Nov 2020 01:19:56 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:19:57 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:20:01 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:20:02 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:20:03 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:20:03 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:20:03 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:20:03 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:20:04 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:20:04 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:20:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:20:04 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca7289d3480a7f27dcc51f696868ab76ca9035d8f944a661bd3e099f1ea78e7`  
		Last Modified: Sat, 21 Nov 2020 01:20:45 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6a7418fece1c5e89caa9a8b68d57bf6b63872ab00bd3859ce7e395553f0407`  
		Last Modified: Sat, 21 Nov 2020 01:20:52 GMT  
		Size: 40.7 MB (40675633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d63f57fc4f6c269ef81dd6fc2a820fdbedd5ab94a5cb506120082ee58054e2`  
		Last Modified: Sat, 21 Nov 2020 01:20:44 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96c54e6fe850cf0048d61bfc9d199e83c415130403528599d7daa7a8540b8b4`  
		Last Modified: Sat, 21 Nov 2020 01:20:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a065ffea4fd3691a75fc16152bada39181b6292a75158a7a75b6d365badc4b60`  
		Last Modified: Sat, 21 Nov 2020 01:20:45 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.10` - linux; arm variant v6

```console
$ docker pull consul@sha256:9898e52e14bff1b3253c7c2e55f5d96c0b811996d660b95c9bbbe17c3924e5b2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39188612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dd65b663c29d650428766e072216c95f4bd8175f4d84dac1b503cc28b136f26`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:17:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:51:34 GMT
ENV CONSUL_VERSION=1.7.10
# Sat, 21 Nov 2020 01:51:35 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:51:37 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:51:45 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:51:47 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:51:49 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:51:50 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:51:50 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:51:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:51:52 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:51:52 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:51:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:51:53 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1a095f2c01406b324aecee6ea15b9382a7f9d3911742cc95943b482697b9cd`  
		Last Modified: Sat, 21 Nov 2020 01:52:56 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c1d8fd42c534d53d881613da0bb84d8c43286324887e006b1b7546ac962b65`  
		Last Modified: Sat, 21 Nov 2020 01:53:06 GMT  
		Size: 36.6 MB (36583407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9a2173853dd15d974475841118cbd7e2b13753d79b5c5b2594bfbef4214a5f`  
		Last Modified: Sat, 21 Nov 2020 01:52:56 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c92bac46c11832762dc2ff097f7722ebd2214322f1f27e7145ac1b5368c2a2`  
		Last Modified: Sat, 21 Nov 2020 01:52:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99776bd6406ac1737981c6af30b75ae07dc17d3d0ba2486fb5d2400f6fedebe7`  
		Last Modified: Sat, 21 Nov 2020 01:52:56 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.10` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:18e46ed1d4d6cbecfca7efbb99a6004d251e53ad1fd3b09ef568c78092aaa232
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.4 MB (39412443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:459b7ea4c4a47d0867cdbb6f9f6345ba9d98569bc13744b5a414d38f17419cff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:42:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:40:35 GMT
ENV CONSUL_VERSION=1.7.10
# Sat, 21 Nov 2020 01:40:37 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:40:40 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:40:47 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:40:50 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:40:52 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:40:52 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:40:53 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:40:54 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:40:54 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:40:55 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:40:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:40:59 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ca11a9c4f0e01c15269e1a922b3e85cace4c6a4e8012fe46d991c3b631543b`  
		Last Modified: Sat, 21 Nov 2020 01:41:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0deadfb700fc32b539eb184f000ab8428f2e3949738e1395648a45ab6b322a2`  
		Last Modified: Sat, 21 Nov 2020 01:42:08 GMT  
		Size: 36.7 MB (36702593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be84067000b0818bb382343e10626a5a994433c7709d998bfd0fd4f72899e175`  
		Last Modified: Sat, 21 Nov 2020 01:41:59 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2515b9e6d5bca0056bbc4fa69d34ec0bf6e33aa2b86357cc377bda959870c449`  
		Last Modified: Sat, 21 Nov 2020 01:41:59 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c666cac88ee672bc0f44329987bf2a1bc19238d7c54b4e2bd428726f9bff8cd0`  
		Last Modified: Sat, 21 Nov 2020 01:41:59 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.10` - linux; 386

```console
$ docker pull consul@sha256:9060331ac68bc5b49ca118d89b3de037f26d930318384931d8ddae9fdac3689a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42273476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5388bbbe3074d5368f55e8be06633a0207adc15d8b1ed956b25f4932e74d47d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:38:55 GMT
ENV CONSUL_VERSION=1.7.10
# Sat, 21 Nov 2020 01:38:55 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:38:56 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:39:03 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:39:04 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:39:05 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:39:05 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:39:05 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:39:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:39:06 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:39:06 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:39:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:39:07 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad9d9e88674a9ee11182151110497f18d229130a39fa8c6afa877d3f68d7211`  
		Last Modified: Sat, 21 Nov 2020 01:39:49 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c3807ca6a52a3d92cceb7f8c1c3ecd3a0e3bebfcf603fc0e1f18ab493350b3`  
		Last Modified: Sat, 21 Nov 2020 01:40:00 GMT  
		Size: 39.5 MB (39478832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f655fb0d3f657436baef11ac6955a8e4d91c3f95bc563042c8e3ee4a83dca2f`  
		Last Modified: Sat, 21 Nov 2020 01:39:49 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8581f6b37196be59e34bc65d25f14344d505b62347fd78de5598bffac35f0c0`  
		Last Modified: Sat, 21 Nov 2020 01:39:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b6f208b77ae07b8b434483ec34c407e10c1b89b132f816cae1a8d498c9fb92`  
		Last Modified: Sat, 21 Nov 2020 01:39:49 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8`

```console
$ docker pull consul@sha256:795445157deb9929b496823e00ed4afb6386055df0e239656bc36ae93d3dddeb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8` - linux; amd64

```console
$ docker pull consul@sha256:d277da56be6d205f561d4d8f45cd816ba2a2765562e2af4efd6693603f56a6b4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46843780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98d273eafda106d20a7c1d0fefcbd384bce7bf3f3d893bf4df40cd63c1330e6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:17:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:19:42 GMT
ENV CONSUL_VERSION=1.8.6
# Sat, 21 Nov 2020 01:19:42 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:19:43 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:19:47 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:19:48 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:19:49 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:19:49 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:19:50 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:19:50 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:19:50 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:19:50 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:19:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:19:51 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f1655ebbbcf610ec26650e0a5bfbf01e8c8ec853ad79797c66b180694673dd`  
		Last Modified: Sat, 21 Nov 2020 01:20:31 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee154555a64570b357e4fe60e60cd9547ac30f83463032fe2286c31047b3f4bb`  
		Last Modified: Sat, 21 Nov 2020 01:20:38 GMT  
		Size: 44.0 MB (44043685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96cd08dca5dfbb66f38c979690b1c612a60726d7ca09186114ba61e5b7a40ab`  
		Last Modified: Sat, 21 Nov 2020 01:20:32 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce97f60b83a621eb7d0f684527052892493786242629445587cd4fb1d0b9419`  
		Last Modified: Sat, 21 Nov 2020 01:20:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719d1014c53db9801d3ec060ef185b952a206f1e302e23697bd8c0917d1accfc`  
		Last Modified: Sat, 21 Nov 2020 01:20:31 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm variant v6

```console
$ docker pull consul@sha256:30ce10937e1d673c8242958397d168a6d9a71ee2e3488b2fbca16af75338c706
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42106096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cee4d822f21c5fb9c35b91eaeeea482f8cbf9ed84ca90b5e35989edff35fbb10`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:17:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:51:02 GMT
ENV CONSUL_VERSION=1.8.6
# Sat, 21 Nov 2020 01:51:03 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:51:05 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:51:17 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:51:19 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:51:22 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:51:22 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:51:23 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:51:24 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:51:24 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:51:25 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:51:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:51:27 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:384109437fd92f8b9265dc381f1089c20ca2603e336a675d7bd58e3191eafd16`  
		Last Modified: Sat, 21 Nov 2020 01:52:36 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ae8e56ff7b1d183cb864e12d05ddb1e77df7af34e361a4185315c3c85922a5`  
		Last Modified: Sat, 21 Nov 2020 01:52:47 GMT  
		Size: 39.5 MB (39500891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef12435db2335bf36731672017bb9572a1265b3a52ed5827922df4c311962933`  
		Last Modified: Sat, 21 Nov 2020 01:52:36 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c3fd0fd13c7db56f4ad43051efc5b427090edd08ce26c6e2d1213dae3a1bd`  
		Last Modified: Sat, 21 Nov 2020 01:52:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a1bdd705ca3038315b24920dfca3ced76e40c66bea8a70a8b84c6e11777f7f`  
		Last Modified: Sat, 21 Nov 2020 01:52:36 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:060e41ee571dc8c701f386868dd7b7fc2dc3105e62f83966815608a43bbf9e3d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42279876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b53eface40401e9c8fcfb315dd1b0a5d964592eac19ad1c0bef0d2919f1cb6a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:42:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:40:04 GMT
ENV CONSUL_VERSION=1.8.6
# Sat, 21 Nov 2020 01:40:05 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:40:07 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:40:14 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:40:16 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:40:19 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:40:19 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:40:20 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:40:21 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:40:22 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:40:22 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:40:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:40:27 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48f31e847d124c01a2f9c8776d3fc597739c8f02f7d18e1f16b476a0cb491e4`  
		Last Modified: Sat, 21 Nov 2020 01:41:41 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1e829303c21b36a12039c446b8aef07c347401504e6d94c8c8af00f4111eff`  
		Last Modified: Sat, 21 Nov 2020 01:41:50 GMT  
		Size: 39.6 MB (39570023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ceaca592f0142a3cca6fa64bd59e9fe13a8aa84e3c73be6d6316ee81eae2b58`  
		Last Modified: Sat, 21 Nov 2020 01:41:40 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703f0c7f3af2a729d9c92c7a9cffdc2b0cb3a7399ed0b51febcdc28ae6c5c828`  
		Last Modified: Sat, 21 Nov 2020 01:41:41 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7965b226005be1e899999da5778b410df38621c8ca1d1cffa1033539d9f9ba4`  
		Last Modified: Sat, 21 Nov 2020 01:41:41 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; 386

```console
$ docker pull consul@sha256:84ae85b48c8d01fce5cc0e9a6e90e9f8afcf43489c397a86af1094e1edcbb979
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.4 MB (46352079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:138cc84a33f3f503a4f09b51b0c3e2ed7fe7f7d6fb2a0a76dc1aed4a30c4c2e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:38:31 GMT
ENV CONSUL_VERSION=1.8.6
# Sat, 21 Nov 2020 01:38:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:38:33 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:38:41 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:38:42 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:38:44 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:38:44 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:38:44 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:38:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:38:45 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:38:45 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:38:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:38:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f7ea6bb49fcd83fa1e2532a46fa73673811b4f190eabbeac27b70126e99483`  
		Last Modified: Sat, 21 Nov 2020 01:39:33 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f5b10ad85a8ca78f92681700a4adf4286665337db08649aade4832e289c1b1`  
		Last Modified: Sat, 21 Nov 2020 01:39:42 GMT  
		Size: 43.6 MB (43557436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc233fbc0a691dfc0d0d6632924d73a80241aace4095d2562084aada2f889003`  
		Last Modified: Sat, 21 Nov 2020 01:39:33 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803b2f813151022af8a8d729fd038d6d97deeb7edf8cda7cd53b6d584074f09d`  
		Last Modified: Sat, 21 Nov 2020 01:39:33 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fb85334aeb38ba47abe71d6bafa659b496f04bb6b2195305ef4dcafbe7929e`  
		Last Modified: Sat, 21 Nov 2020 01:39:33 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8.6`

```console
$ docker pull consul@sha256:795445157deb9929b496823e00ed4afb6386055df0e239656bc36ae93d3dddeb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8.6` - linux; amd64

```console
$ docker pull consul@sha256:d277da56be6d205f561d4d8f45cd816ba2a2765562e2af4efd6693603f56a6b4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46843780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98d273eafda106d20a7c1d0fefcbd384bce7bf3f3d893bf4df40cd63c1330e6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:17:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:19:42 GMT
ENV CONSUL_VERSION=1.8.6
# Sat, 21 Nov 2020 01:19:42 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:19:43 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:19:47 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:19:48 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:19:49 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:19:49 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:19:50 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:19:50 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:19:50 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:19:50 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:19:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:19:51 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f1655ebbbcf610ec26650e0a5bfbf01e8c8ec853ad79797c66b180694673dd`  
		Last Modified: Sat, 21 Nov 2020 01:20:31 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee154555a64570b357e4fe60e60cd9547ac30f83463032fe2286c31047b3f4bb`  
		Last Modified: Sat, 21 Nov 2020 01:20:38 GMT  
		Size: 44.0 MB (44043685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96cd08dca5dfbb66f38c979690b1c612a60726d7ca09186114ba61e5b7a40ab`  
		Last Modified: Sat, 21 Nov 2020 01:20:32 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce97f60b83a621eb7d0f684527052892493786242629445587cd4fb1d0b9419`  
		Last Modified: Sat, 21 Nov 2020 01:20:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719d1014c53db9801d3ec060ef185b952a206f1e302e23697bd8c0917d1accfc`  
		Last Modified: Sat, 21 Nov 2020 01:20:31 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.6` - linux; arm variant v6

```console
$ docker pull consul@sha256:30ce10937e1d673c8242958397d168a6d9a71ee2e3488b2fbca16af75338c706
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42106096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cee4d822f21c5fb9c35b91eaeeea482f8cbf9ed84ca90b5e35989edff35fbb10`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:17:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:51:02 GMT
ENV CONSUL_VERSION=1.8.6
# Sat, 21 Nov 2020 01:51:03 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:51:05 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:51:17 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:51:19 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:51:22 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:51:22 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:51:23 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:51:24 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:51:24 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:51:25 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:51:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:51:27 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:384109437fd92f8b9265dc381f1089c20ca2603e336a675d7bd58e3191eafd16`  
		Last Modified: Sat, 21 Nov 2020 01:52:36 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ae8e56ff7b1d183cb864e12d05ddb1e77df7af34e361a4185315c3c85922a5`  
		Last Modified: Sat, 21 Nov 2020 01:52:47 GMT  
		Size: 39.5 MB (39500891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef12435db2335bf36731672017bb9572a1265b3a52ed5827922df4c311962933`  
		Last Modified: Sat, 21 Nov 2020 01:52:36 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c3fd0fd13c7db56f4ad43051efc5b427090edd08ce26c6e2d1213dae3a1bd`  
		Last Modified: Sat, 21 Nov 2020 01:52:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a1bdd705ca3038315b24920dfca3ced76e40c66bea8a70a8b84c6e11777f7f`  
		Last Modified: Sat, 21 Nov 2020 01:52:36 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.6` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:060e41ee571dc8c701f386868dd7b7fc2dc3105e62f83966815608a43bbf9e3d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42279876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b53eface40401e9c8fcfb315dd1b0a5d964592eac19ad1c0bef0d2919f1cb6a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:42:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:40:04 GMT
ENV CONSUL_VERSION=1.8.6
# Sat, 21 Nov 2020 01:40:05 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:40:07 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:40:14 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:40:16 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:40:19 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:40:19 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:40:20 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:40:21 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:40:22 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:40:22 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:40:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:40:27 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48f31e847d124c01a2f9c8776d3fc597739c8f02f7d18e1f16b476a0cb491e4`  
		Last Modified: Sat, 21 Nov 2020 01:41:41 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1e829303c21b36a12039c446b8aef07c347401504e6d94c8c8af00f4111eff`  
		Last Modified: Sat, 21 Nov 2020 01:41:50 GMT  
		Size: 39.6 MB (39570023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ceaca592f0142a3cca6fa64bd59e9fe13a8aa84e3c73be6d6316ee81eae2b58`  
		Last Modified: Sat, 21 Nov 2020 01:41:40 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703f0c7f3af2a729d9c92c7a9cffdc2b0cb3a7399ed0b51febcdc28ae6c5c828`  
		Last Modified: Sat, 21 Nov 2020 01:41:41 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7965b226005be1e899999da5778b410df38621c8ca1d1cffa1033539d9f9ba4`  
		Last Modified: Sat, 21 Nov 2020 01:41:41 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.6` - linux; 386

```console
$ docker pull consul@sha256:84ae85b48c8d01fce5cc0e9a6e90e9f8afcf43489c397a86af1094e1edcbb979
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.4 MB (46352079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:138cc84a33f3f503a4f09b51b0c3e2ed7fe7f7d6fb2a0a76dc1aed4a30c4c2e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:38:31 GMT
ENV CONSUL_VERSION=1.8.6
# Sat, 21 Nov 2020 01:38:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:38:33 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:38:41 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:38:42 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:38:44 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:38:44 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:38:44 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:38:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:38:45 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:38:45 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:38:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:38:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f7ea6bb49fcd83fa1e2532a46fa73673811b4f190eabbeac27b70126e99483`  
		Last Modified: Sat, 21 Nov 2020 01:39:33 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f5b10ad85a8ca78f92681700a4adf4286665337db08649aade4832e289c1b1`  
		Last Modified: Sat, 21 Nov 2020 01:39:42 GMT  
		Size: 43.6 MB (43557436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc233fbc0a691dfc0d0d6632924d73a80241aace4095d2562084aada2f889003`  
		Last Modified: Sat, 21 Nov 2020 01:39:33 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803b2f813151022af8a8d729fd038d6d97deeb7edf8cda7cd53b6d584074f09d`  
		Last Modified: Sat, 21 Nov 2020 01:39:33 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fb85334aeb38ba47abe71d6bafa659b496f04bb6b2195305ef4dcafbe7929e`  
		Last Modified: Sat, 21 Nov 2020 01:39:33 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8.7-beta1`

```console
$ docker pull consul@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `consul:1.9`

```console
$ docker pull consul@sha256:6729ed37212457d5f10047deac649ff7e055ced4405398d560593fbfa364d854
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9` - linux; amd64

```console
$ docker pull consul@sha256:ac53c00d84995919d5aa1c2ae35a91cee9290a94565abf586adfd4055499b13b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45904190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c239afe7006ea6f61ef8f831dece8e59dd43483f68b08f752569b2cf8cfc2bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:17:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 25 Nov 2020 00:28:51 GMT
ENV CONSUL_VERSION=1.9.0
# Wed, 25 Nov 2020 00:28:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 25 Nov 2020 00:28:52 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 25 Nov 2020 00:28:57 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 25 Nov 2020 00:28:58 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 25 Nov 2020 00:28:59 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 Nov 2020 00:28:59 GMT
VOLUME [/consul/data]
# Wed, 25 Nov 2020 00:28:59 GMT
EXPOSE 8300
# Wed, 25 Nov 2020 00:28:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 25 Nov 2020 00:29:00 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 25 Nov 2020 00:29:00 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 25 Nov 2020 00:29:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 00:29:00 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e15e1d587e61c76b419da1505677b8df056a305abaeacba7aae92190b1423b`  
		Last Modified: Wed, 25 Nov 2020 00:29:21 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6d13050091293a8f40d89e7d157cf6f880e81eba6e9e1a98257a5ea4838725`  
		Last Modified: Wed, 25 Nov 2020 00:29:28 GMT  
		Size: 43.1 MB (43104098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd9fbb86a8f901859f680a2024b38edc40db52f0457c65e185757992c5a1368`  
		Last Modified: Wed, 25 Nov 2020 00:29:21 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e582f80d6b3012291ba2df400fca5593734cc8254220e891bac3595f1759a0b1`  
		Last Modified: Wed, 25 Nov 2020 00:29:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b4f4adec89a554af8933aaae1903ffdad7aaaa6aa5fe0746ddbd08d818b7f0`  
		Last Modified: Wed, 25 Nov 2020 00:29:21 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm variant v6

```console
$ docker pull consul@sha256:45629f4f5ed311f73724880098846df68977ea44bfb74197cfb6b40666e1e87a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41177693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a659f752b75b6bf5c28cdf21067ce3e1e53f2fc457a6181331e89cfe7748928`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:17:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 25 Nov 2020 00:49:37 GMT
ENV CONSUL_VERSION=1.9.0
# Wed, 25 Nov 2020 00:49:38 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 25 Nov 2020 00:49:45 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 25 Nov 2020 00:50:04 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 25 Nov 2020 00:50:08 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 25 Nov 2020 00:50:13 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 Nov 2020 00:50:15 GMT
VOLUME [/consul/data]
# Wed, 25 Nov 2020 00:50:17 GMT
EXPOSE 8300
# Wed, 25 Nov 2020 00:50:18 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 25 Nov 2020 00:50:19 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 25 Nov 2020 00:50:21 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 25 Nov 2020 00:50:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 00:50:24 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541d1797ef1170490288147b99ee5d41a948a7f4e79f641fafc5f6fed3d80b38`  
		Last Modified: Wed, 25 Nov 2020 00:51:01 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412943d31f925789bbd6d15ce0453a3b619149b5ab000b93ddf626356ca6e8b5`  
		Last Modified: Wed, 25 Nov 2020 00:51:18 GMT  
		Size: 38.6 MB (38572484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03138968c5fe96a538b0bf6df3091212fd588bcf78dbeb51b3c4dc8d044cfb66`  
		Last Modified: Wed, 25 Nov 2020 00:51:01 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691e110ed2b0a550bf4acbc2e4d169923f3fec45f1fd7020ec1ec81d1fd4fd36`  
		Last Modified: Wed, 25 Nov 2020 00:51:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22af8e92dfceb088c9546e2566415d438f1874b57b0ed365044b1a67d27bae92`  
		Last Modified: Wed, 25 Nov 2020 00:51:02 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:1012b86c1b4f0c40be0449c239cdd6f1adfbf34ce7a6ccf5903245f890ff677d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.4 MB (41394856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82b6a768f504e8509835bc02fa5a484eba01a4389908306659d0829492078a5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:42:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 25 Nov 2020 00:39:32 GMT
ENV CONSUL_VERSION=1.9.0
# Wed, 25 Nov 2020 00:39:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 25 Nov 2020 00:39:34 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 25 Nov 2020 00:39:43 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 25 Nov 2020 00:39:46 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 25 Nov 2020 00:39:49 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 Nov 2020 00:39:50 GMT
VOLUME [/consul/data]
# Wed, 25 Nov 2020 00:39:50 GMT
EXPOSE 8300
# Wed, 25 Nov 2020 00:39:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 25 Nov 2020 00:39:52 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 25 Nov 2020 00:39:53 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 25 Nov 2020 00:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 00:39:54 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4785ac6d608aceb5c11acbff79d38f8310fe7ea952dbc1fe0f16ee4157bb7fb`  
		Last Modified: Wed, 25 Nov 2020 00:40:25 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda07bb163802553eb787a581765163466d5b9d9fcdf8079b1f9a15d30a000ed`  
		Last Modified: Wed, 25 Nov 2020 00:40:35 GMT  
		Size: 38.7 MB (38685008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbadd110c842ac687b4e011516cbb85cb5351ed410ffc7d9ce8e29d6a81b980a`  
		Last Modified: Wed, 25 Nov 2020 00:40:25 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044fc41f7bedc3f964514a77a849e654c872f9a7ff56dedee9354f0931c41552`  
		Last Modified: Wed, 25 Nov 2020 00:40:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261b79696f40f83b31ed9b8fa30c52dc07c56f018ae83b8e705fae062b94b651`  
		Last Modified: Wed, 25 Nov 2020 00:40:26 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; 386

```console
$ docker pull consul@sha256:3ad6148e3cdb242420b209f4d1fe73da7c23f2c78598dbb3df16f6538d5a013a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45231403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:addffb46e74179410991b94d4784f09f5e804e3345dea67754c93b743b861fbc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 25 Nov 2020 00:38:31 GMT
ENV CONSUL_VERSION=1.9.0
# Wed, 25 Nov 2020 00:38:31 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 25 Nov 2020 00:38:32 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 25 Nov 2020 00:38:38 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 25 Nov 2020 00:38:39 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 25 Nov 2020 00:38:39 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 Nov 2020 00:38:40 GMT
VOLUME [/consul/data]
# Wed, 25 Nov 2020 00:38:40 GMT
EXPOSE 8300
# Wed, 25 Nov 2020 00:38:40 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 25 Nov 2020 00:38:40 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 25 Nov 2020 00:38:41 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 25 Nov 2020 00:38:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 00:38:41 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b670227cf5b0369dec1890afd49daa761d5219f770e6e1717eeb94aa0d30d795`  
		Last Modified: Wed, 25 Nov 2020 00:39:03 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886f4ead96bdf58722ac9a1bb62e065252db84d364caac2f2f162484607b9679`  
		Last Modified: Wed, 25 Nov 2020 00:39:12 GMT  
		Size: 42.4 MB (42436764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9099eaffdcf30a6fc42310fad858f1210dc9a72b912f3867f84114f14283e4b1`  
		Last Modified: Wed, 25 Nov 2020 00:39:03 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60de6fed51016b0bc661d53792674a602f12405b5ee4fa32ff4760a2c97fd0a`  
		Last Modified: Wed, 25 Nov 2020 00:39:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1722523c085b312cc345217410e18206bcf15369b2bb5c423315508580a7e0`  
		Last Modified: Wed, 25 Nov 2020 00:39:03 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9.0`

```console
$ docker pull consul@sha256:6729ed37212457d5f10047deac649ff7e055ced4405398d560593fbfa364d854
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9.0` - linux; amd64

```console
$ docker pull consul@sha256:ac53c00d84995919d5aa1c2ae35a91cee9290a94565abf586adfd4055499b13b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45904190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c239afe7006ea6f61ef8f831dece8e59dd43483f68b08f752569b2cf8cfc2bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:17:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 25 Nov 2020 00:28:51 GMT
ENV CONSUL_VERSION=1.9.0
# Wed, 25 Nov 2020 00:28:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 25 Nov 2020 00:28:52 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 25 Nov 2020 00:28:57 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 25 Nov 2020 00:28:58 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 25 Nov 2020 00:28:59 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 Nov 2020 00:28:59 GMT
VOLUME [/consul/data]
# Wed, 25 Nov 2020 00:28:59 GMT
EXPOSE 8300
# Wed, 25 Nov 2020 00:28:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 25 Nov 2020 00:29:00 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 25 Nov 2020 00:29:00 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 25 Nov 2020 00:29:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 00:29:00 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e15e1d587e61c76b419da1505677b8df056a305abaeacba7aae92190b1423b`  
		Last Modified: Wed, 25 Nov 2020 00:29:21 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6d13050091293a8f40d89e7d157cf6f880e81eba6e9e1a98257a5ea4838725`  
		Last Modified: Wed, 25 Nov 2020 00:29:28 GMT  
		Size: 43.1 MB (43104098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd9fbb86a8f901859f680a2024b38edc40db52f0457c65e185757992c5a1368`  
		Last Modified: Wed, 25 Nov 2020 00:29:21 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e582f80d6b3012291ba2df400fca5593734cc8254220e891bac3595f1759a0b1`  
		Last Modified: Wed, 25 Nov 2020 00:29:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b4f4adec89a554af8933aaae1903ffdad7aaaa6aa5fe0746ddbd08d818b7f0`  
		Last Modified: Wed, 25 Nov 2020 00:29:21 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.0` - linux; arm variant v6

```console
$ docker pull consul@sha256:45629f4f5ed311f73724880098846df68977ea44bfb74197cfb6b40666e1e87a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41177693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a659f752b75b6bf5c28cdf21067ce3e1e53f2fc457a6181331e89cfe7748928`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:17:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 25 Nov 2020 00:49:37 GMT
ENV CONSUL_VERSION=1.9.0
# Wed, 25 Nov 2020 00:49:38 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 25 Nov 2020 00:49:45 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 25 Nov 2020 00:50:04 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 25 Nov 2020 00:50:08 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 25 Nov 2020 00:50:13 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 Nov 2020 00:50:15 GMT
VOLUME [/consul/data]
# Wed, 25 Nov 2020 00:50:17 GMT
EXPOSE 8300
# Wed, 25 Nov 2020 00:50:18 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 25 Nov 2020 00:50:19 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 25 Nov 2020 00:50:21 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 25 Nov 2020 00:50:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 00:50:24 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541d1797ef1170490288147b99ee5d41a948a7f4e79f641fafc5f6fed3d80b38`  
		Last Modified: Wed, 25 Nov 2020 00:51:01 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412943d31f925789bbd6d15ce0453a3b619149b5ab000b93ddf626356ca6e8b5`  
		Last Modified: Wed, 25 Nov 2020 00:51:18 GMT  
		Size: 38.6 MB (38572484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03138968c5fe96a538b0bf6df3091212fd588bcf78dbeb51b3c4dc8d044cfb66`  
		Last Modified: Wed, 25 Nov 2020 00:51:01 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691e110ed2b0a550bf4acbc2e4d169923f3fec45f1fd7020ec1ec81d1fd4fd36`  
		Last Modified: Wed, 25 Nov 2020 00:51:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22af8e92dfceb088c9546e2566415d438f1874b57b0ed365044b1a67d27bae92`  
		Last Modified: Wed, 25 Nov 2020 00:51:02 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.0` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:1012b86c1b4f0c40be0449c239cdd6f1adfbf34ce7a6ccf5903245f890ff677d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.4 MB (41394856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82b6a768f504e8509835bc02fa5a484eba01a4389908306659d0829492078a5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:42:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 25 Nov 2020 00:39:32 GMT
ENV CONSUL_VERSION=1.9.0
# Wed, 25 Nov 2020 00:39:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 25 Nov 2020 00:39:34 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 25 Nov 2020 00:39:43 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 25 Nov 2020 00:39:46 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 25 Nov 2020 00:39:49 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 Nov 2020 00:39:50 GMT
VOLUME [/consul/data]
# Wed, 25 Nov 2020 00:39:50 GMT
EXPOSE 8300
# Wed, 25 Nov 2020 00:39:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 25 Nov 2020 00:39:52 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 25 Nov 2020 00:39:53 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 25 Nov 2020 00:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 00:39:54 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4785ac6d608aceb5c11acbff79d38f8310fe7ea952dbc1fe0f16ee4157bb7fb`  
		Last Modified: Wed, 25 Nov 2020 00:40:25 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda07bb163802553eb787a581765163466d5b9d9fcdf8079b1f9a15d30a000ed`  
		Last Modified: Wed, 25 Nov 2020 00:40:35 GMT  
		Size: 38.7 MB (38685008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbadd110c842ac687b4e011516cbb85cb5351ed410ffc7d9ce8e29d6a81b980a`  
		Last Modified: Wed, 25 Nov 2020 00:40:25 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044fc41f7bedc3f964514a77a849e654c872f9a7ff56dedee9354f0931c41552`  
		Last Modified: Wed, 25 Nov 2020 00:40:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261b79696f40f83b31ed9b8fa30c52dc07c56f018ae83b8e705fae062b94b651`  
		Last Modified: Wed, 25 Nov 2020 00:40:26 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.0` - linux; 386

```console
$ docker pull consul@sha256:3ad6148e3cdb242420b209f4d1fe73da7c23f2c78598dbb3df16f6538d5a013a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45231403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:addffb46e74179410991b94d4784f09f5e804e3345dea67754c93b743b861fbc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 25 Nov 2020 00:38:31 GMT
ENV CONSUL_VERSION=1.9.0
# Wed, 25 Nov 2020 00:38:31 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 25 Nov 2020 00:38:32 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 25 Nov 2020 00:38:38 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 25 Nov 2020 00:38:39 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 25 Nov 2020 00:38:39 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 Nov 2020 00:38:40 GMT
VOLUME [/consul/data]
# Wed, 25 Nov 2020 00:38:40 GMT
EXPOSE 8300
# Wed, 25 Nov 2020 00:38:40 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 25 Nov 2020 00:38:40 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 25 Nov 2020 00:38:41 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 25 Nov 2020 00:38:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 00:38:41 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b670227cf5b0369dec1890afd49daa761d5219f770e6e1717eeb94aa0d30d795`  
		Last Modified: Wed, 25 Nov 2020 00:39:03 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886f4ead96bdf58722ac9a1bb62e065252db84d364caac2f2f162484607b9679`  
		Last Modified: Wed, 25 Nov 2020 00:39:12 GMT  
		Size: 42.4 MB (42436764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9099eaffdcf30a6fc42310fad858f1210dc9a72b912f3867f84114f14283e4b1`  
		Last Modified: Wed, 25 Nov 2020 00:39:03 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60de6fed51016b0bc661d53792674a602f12405b5ee4fa32ff4760a2c97fd0a`  
		Last Modified: Wed, 25 Nov 2020 00:39:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1722523c085b312cc345217410e18206bcf15369b2bb5c423315508580a7e0`  
		Last Modified: Wed, 25 Nov 2020 00:39:03 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:6729ed37212457d5f10047deac649ff7e055ced4405398d560593fbfa364d854
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:ac53c00d84995919d5aa1c2ae35a91cee9290a94565abf586adfd4055499b13b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45904190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c239afe7006ea6f61ef8f831dece8e59dd43483f68b08f752569b2cf8cfc2bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:17:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 25 Nov 2020 00:28:51 GMT
ENV CONSUL_VERSION=1.9.0
# Wed, 25 Nov 2020 00:28:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 25 Nov 2020 00:28:52 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 25 Nov 2020 00:28:57 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 25 Nov 2020 00:28:58 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 25 Nov 2020 00:28:59 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 Nov 2020 00:28:59 GMT
VOLUME [/consul/data]
# Wed, 25 Nov 2020 00:28:59 GMT
EXPOSE 8300
# Wed, 25 Nov 2020 00:28:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 25 Nov 2020 00:29:00 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 25 Nov 2020 00:29:00 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 25 Nov 2020 00:29:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 00:29:00 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e15e1d587e61c76b419da1505677b8df056a305abaeacba7aae92190b1423b`  
		Last Modified: Wed, 25 Nov 2020 00:29:21 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6d13050091293a8f40d89e7d157cf6f880e81eba6e9e1a98257a5ea4838725`  
		Last Modified: Wed, 25 Nov 2020 00:29:28 GMT  
		Size: 43.1 MB (43104098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd9fbb86a8f901859f680a2024b38edc40db52f0457c65e185757992c5a1368`  
		Last Modified: Wed, 25 Nov 2020 00:29:21 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e582f80d6b3012291ba2df400fca5593734cc8254220e891bac3595f1759a0b1`  
		Last Modified: Wed, 25 Nov 2020 00:29:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b4f4adec89a554af8933aaae1903ffdad7aaaa6aa5fe0746ddbd08d818b7f0`  
		Last Modified: Wed, 25 Nov 2020 00:29:21 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:45629f4f5ed311f73724880098846df68977ea44bfb74197cfb6b40666e1e87a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41177693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a659f752b75b6bf5c28cdf21067ce3e1e53f2fc457a6181331e89cfe7748928`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:17:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 25 Nov 2020 00:49:37 GMT
ENV CONSUL_VERSION=1.9.0
# Wed, 25 Nov 2020 00:49:38 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 25 Nov 2020 00:49:45 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 25 Nov 2020 00:50:04 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 25 Nov 2020 00:50:08 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 25 Nov 2020 00:50:13 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 Nov 2020 00:50:15 GMT
VOLUME [/consul/data]
# Wed, 25 Nov 2020 00:50:17 GMT
EXPOSE 8300
# Wed, 25 Nov 2020 00:50:18 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 25 Nov 2020 00:50:19 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 25 Nov 2020 00:50:21 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 25 Nov 2020 00:50:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 00:50:24 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541d1797ef1170490288147b99ee5d41a948a7f4e79f641fafc5f6fed3d80b38`  
		Last Modified: Wed, 25 Nov 2020 00:51:01 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412943d31f925789bbd6d15ce0453a3b619149b5ab000b93ddf626356ca6e8b5`  
		Last Modified: Wed, 25 Nov 2020 00:51:18 GMT  
		Size: 38.6 MB (38572484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03138968c5fe96a538b0bf6df3091212fd588bcf78dbeb51b3c4dc8d044cfb66`  
		Last Modified: Wed, 25 Nov 2020 00:51:01 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691e110ed2b0a550bf4acbc2e4d169923f3fec45f1fd7020ec1ec81d1fd4fd36`  
		Last Modified: Wed, 25 Nov 2020 00:51:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22af8e92dfceb088c9546e2566415d438f1874b57b0ed365044b1a67d27bae92`  
		Last Modified: Wed, 25 Nov 2020 00:51:02 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:1012b86c1b4f0c40be0449c239cdd6f1adfbf34ce7a6ccf5903245f890ff677d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.4 MB (41394856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82b6a768f504e8509835bc02fa5a484eba01a4389908306659d0829492078a5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:42:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 25 Nov 2020 00:39:32 GMT
ENV CONSUL_VERSION=1.9.0
# Wed, 25 Nov 2020 00:39:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 25 Nov 2020 00:39:34 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 25 Nov 2020 00:39:43 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 25 Nov 2020 00:39:46 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 25 Nov 2020 00:39:49 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 Nov 2020 00:39:50 GMT
VOLUME [/consul/data]
# Wed, 25 Nov 2020 00:39:50 GMT
EXPOSE 8300
# Wed, 25 Nov 2020 00:39:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 25 Nov 2020 00:39:52 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 25 Nov 2020 00:39:53 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 25 Nov 2020 00:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 00:39:54 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4785ac6d608aceb5c11acbff79d38f8310fe7ea952dbc1fe0f16ee4157bb7fb`  
		Last Modified: Wed, 25 Nov 2020 00:40:25 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda07bb163802553eb787a581765163466d5b9d9fcdf8079b1f9a15d30a000ed`  
		Last Modified: Wed, 25 Nov 2020 00:40:35 GMT  
		Size: 38.7 MB (38685008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbadd110c842ac687b4e011516cbb85cb5351ed410ffc7d9ce8e29d6a81b980a`  
		Last Modified: Wed, 25 Nov 2020 00:40:25 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044fc41f7bedc3f964514a77a849e654c872f9a7ff56dedee9354f0931c41552`  
		Last Modified: Wed, 25 Nov 2020 00:40:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261b79696f40f83b31ed9b8fa30c52dc07c56f018ae83b8e705fae062b94b651`  
		Last Modified: Wed, 25 Nov 2020 00:40:26 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:3ad6148e3cdb242420b209f4d1fe73da7c23f2c78598dbb3df16f6538d5a013a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45231403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:addffb46e74179410991b94d4784f09f5e804e3345dea67754c93b743b861fbc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 25 Nov 2020 00:38:31 GMT
ENV CONSUL_VERSION=1.9.0
# Wed, 25 Nov 2020 00:38:31 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 25 Nov 2020 00:38:32 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 25 Nov 2020 00:38:38 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 25 Nov 2020 00:38:39 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 25 Nov 2020 00:38:39 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 Nov 2020 00:38:40 GMT
VOLUME [/consul/data]
# Wed, 25 Nov 2020 00:38:40 GMT
EXPOSE 8300
# Wed, 25 Nov 2020 00:38:40 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 25 Nov 2020 00:38:40 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 25 Nov 2020 00:38:41 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 25 Nov 2020 00:38:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 00:38:41 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b670227cf5b0369dec1890afd49daa761d5219f770e6e1717eeb94aa0d30d795`  
		Last Modified: Wed, 25 Nov 2020 00:39:03 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886f4ead96bdf58722ac9a1bb62e065252db84d364caac2f2f162484607b9679`  
		Last Modified: Wed, 25 Nov 2020 00:39:12 GMT  
		Size: 42.4 MB (42436764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9099eaffdcf30a6fc42310fad858f1210dc9a72b912f3867f84114f14283e4b1`  
		Last Modified: Wed, 25 Nov 2020 00:39:03 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60de6fed51016b0bc661d53792674a602f12405b5ee4fa32ff4760a2c97fd0a`  
		Last Modified: Wed, 25 Nov 2020 00:39:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1722523c085b312cc345217410e18206bcf15369b2bb5c423315508580a7e0`  
		Last Modified: Wed, 25 Nov 2020 00:39:03 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
