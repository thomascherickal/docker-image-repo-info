## `consul:latest`

```console
$ docker pull consul@sha256:cc7b4d6ab8f9566698d427a0bf15a5131841b02d7288588b71e5854c37bd98ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:ee35e3fd2b35d790a533464e50f6fe43aafa0e3806354cc0265d95b35f7400e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45570396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:958f2bba75997fafbccecdfb4b4300dfc99c64fd56d2833f840768f730b1052e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:55:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 18:10:35 GMT
ENV CONSUL_VERSION=1.9.1
# Sat, 12 Dec 2020 18:10:35 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 18:10:36 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 18:10:41 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 18:10:42 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 18:10:43 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 18:10:43 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 18:10:43 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 18:10:43 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 18:10:43 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 18:10:44 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 18:10:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 18:10:44 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a3cabec490762fe7c1682455f9a2b2e320ceae8da91eb35b37c39b5783e403`  
		Last Modified: Sat, 12 Dec 2020 18:11:25 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0538a1f915b778b756a74592840a68bf5b6a5bc60ab99f8f856079acf8c21c`  
		Last Modified: Sat, 12 Dec 2020 18:11:32 GMT  
		Size: 42.8 MB (42770214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f6bd70bdf9ab843e9922f4b141362c6f21dd373b57f1e0d9e05be832275994`  
		Last Modified: Sat, 12 Dec 2020 18:11:25 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7e79697988f100cf30f3f1e08e02fc6c521d767147c9d4df66e349147dddba`  
		Last Modified: Sat, 12 Dec 2020 18:11:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce30221736f3aa7199e6ed008bd3220f589bce402fdf97dabc10bf0f59fef5c3`  
		Last Modified: Sat, 12 Dec 2020 18:11:25 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:ba2cf92ad7a299b67b0836ec07dc80362f4e4983ef588cf78778a5c8b1453a55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40832579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41486a63c4ded8d1f8cac34fd763459ae65be3c5802bef1fed8232cc2f8336d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:12:13 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 00:53:40 GMT
ENV CONSUL_VERSION=1.9.1
# Sat, 12 Dec 2020 00:53:42 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 00:53:46 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 00:53:56 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 00:53:58 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 00:54:02 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 00:54:03 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 00:54:04 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 00:54:05 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 00:54:08 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 00:54:12 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 00:54:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 00:54:19 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f07005897aa5ca7dc61824b38a71822bf3c41d8ee1381f410f3cec7e71295e`  
		Last Modified: Sat, 12 Dec 2020 00:56:24 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0abaf0b0db4322f0c362e05a8f33b4bd9459c9e5b10d7fb9460d51bd0aec91`  
		Last Modified: Sat, 12 Dec 2020 00:56:33 GMT  
		Size: 38.2 MB (38227295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd18ac82951699c3cf6a5d413f6934917c183b4e08716016d14566525a71bcd0`  
		Last Modified: Sat, 12 Dec 2020 00:56:24 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5326c928d9eb761f450fad803c5bc4643fa105e666092783558b85557c8b3bc0`  
		Last Modified: Sat, 12 Dec 2020 00:56:24 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48742b61655f27ca3ed3c85be1b091efb7b1e1024749a53d4984a4c1e178bf8d`  
		Last Modified: Sat, 12 Dec 2020 00:56:24 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:01d2cef184a6ff688693974cfcc36c5d92f9a37832381b2a008e460b26d358f0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41052267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e983dda7fd04f095f885f204ae5c644845ca023ce29555418af478cf5d046c7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:36:07 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 14:07:35 GMT
ENV CONSUL_VERSION=1.9.1
# Sat, 12 Dec 2020 14:07:35 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 14:07:37 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 14:07:44 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 14:07:46 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 14:07:50 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 14:07:51 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 14:07:52 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 14:07:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 14:07:55 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 14:07:55 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 14:07:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 14:07:57 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c8060704c53f3ff052629f979f702282b4cdedc728a02c83ddfcb511067de2`  
		Last Modified: Sat, 12 Dec 2020 14:09:08 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40fc274a81c60ca4deddc3eb2021465a3cacb68e5c35024212cf02fa2a3055da`  
		Last Modified: Sat, 12 Dec 2020 14:09:16 GMT  
		Size: 38.3 MB (38342356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421085bf757533067046c72d4f76aa17383fe82a1c5a709df6015e5f3f7a3af3`  
		Last Modified: Sat, 12 Dec 2020 14:09:08 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92d7c3c09e2f09ab13919755506eb2699a0dbcf2b107a570e6bc9ca536be912`  
		Last Modified: Sat, 12 Dec 2020 14:09:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa6ebe29a594ab16a614fc400231c0e5d0b79f316e51ebf17b0ebcdd0db9875`  
		Last Modified: Sat, 12 Dec 2020 14:09:08 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:06faa80f0bfba7962ff496d09fb892760439823eabe40c6915f3a32cce950018
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44903544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd3a426b880d0017fa66288c3a1f92a89a9a425e86cbcda5d66762a0fec10258`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:01:14 GMT
ADD file:8812e502f26af2dc4efdfb7387f8bf99f2a098b6c95b9f6abf900df2ce74e3da in / 
# Fri, 11 Dec 2020 02:01:14 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:57:39 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 16:21:38 GMT
ENV CONSUL_VERSION=1.9.1
# Sat, 12 Dec 2020 16:21:38 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 16:21:39 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 16:21:47 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 16:21:48 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 16:21:49 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 16:21:50 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 16:21:50 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 16:21:50 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 16:21:51 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 16:21:51 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 16:21:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 16:21:52 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b62269920a7a62a905817c7c1b33f33b6e658121e9a054715ff052a23f7de3a0`  
		Last Modified: Fri, 11 Dec 2020 02:01:43 GMT  
		Size: 2.8 MB (2791504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d44decd170c537cbf0169cb6157dbce3addc3082d52007a874f5f02f907ec3`  
		Last Modified: Sat, 12 Dec 2020 16:22:45 GMT  
		Size: 1.2 KB (1228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b95d7a59da7c28695c7b52be91ec48f2abeaf8a7772b472d3422d1c0e7bfbb4`  
		Last Modified: Sat, 12 Dec 2020 16:22:57 GMT  
		Size: 42.1 MB (42108808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e398434dc9091267104c4cc6271516cdff49e87102373432f2294ffa99b3dc2`  
		Last Modified: Sat, 12 Dec 2020 16:22:44 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09c6b429057f7e0f03ee300f359dc209beedaae65ad4733c1006a2552f98ea6`  
		Last Modified: Sat, 12 Dec 2020 16:22:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1977bb69b681a65c762e379e90c09ff9913147a1c76be17b8338df50330aaf2a`  
		Last Modified: Sat, 12 Dec 2020 16:22:45 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
