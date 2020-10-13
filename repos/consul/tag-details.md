<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.6`](#consul16)
-	[`consul:1.6.9`](#consul169)
-	[`consul:1.7`](#consul17)
-	[`consul:1.7.8`](#consul178)
-	[`consul:1.8`](#consul18)
-	[`consul:1.8.4`](#consul184)
-	[`consul:1.9.0-beta`](#consul190-beta)
-	[`consul:1.9.0-beta1`](#consul190-beta1)
-	[`consul:latest`](#consullatest)

## `consul:1.6`

```console
$ docker pull consul@sha256:574cc0884f2a46336d74a027957d9edff7498fd92562bd26530c734ecc0acf32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.6` - linux; amd64

```console
$ docker pull consul@sha256:eddec9d26473fe2e94f4e3bd1b881af9f873dce17f441feaabef2dc531b1b09d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42259611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e74740b420e54b5fabfa7de9085e3f9a92284a068f07e2b2d1ff51da47e8d752`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 21:35:16 GMT
ENV CONSUL_VERSION=1.6.9
# Fri, 11 Sep 2020 21:35:16 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 21:35:17 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 21:35:21 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 21:35:22 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 21:35:23 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 21:35:23 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 21:35:23 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 21:35:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 21:35:23 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 21:35:24 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 21:35:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 21:35:24 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c42497aee15ea85ada3648423d8d60d805b4046840e36e2592010f03b46b5c3`  
		Last Modified: Fri, 11 Sep 2020 21:35:56 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb172b87dfe72a49c6f089cf7da7c050b7da582882d8acf632f5f7912bf3ffa7`  
		Last Modified: Fri, 11 Sep 2020 21:36:01 GMT  
		Size: 39.5 MB (39458832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f80f502d16c7f8614e287d6b921d01d7e0dbd9eb57e6aedaf04567acc00f07`  
		Last Modified: Fri, 11 Sep 2020 21:35:55 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05694da12802199551dded466f04e09ea60449649d97d73f9845a24753edb98d`  
		Last Modified: Fri, 11 Sep 2020 21:35:55 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5013954d81caeedbfde4d469f884e6ec28c3fc8b608b467cd4e34104b573ed6a`  
		Last Modified: Fri, 11 Sep 2020 21:35:55 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; arm variant v6

```console
$ docker pull consul@sha256:d1b234763bc339b9a12a6b9785ed3e72e65b0a6d605bef8891fa5bcdfc49eba0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37937989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:027d81057134e497189496564bbd4c442b07d593dd9c56234c766a3758974827`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:49:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 20:50:27 GMT
ENV CONSUL_VERSION=1.6.9
# Fri, 11 Sep 2020 20:50:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 20:50:31 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 20:50:40 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 20:50:43 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 20:50:45 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 20:50:46 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 20:50:47 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 20:50:50 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 20:50:51 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 20:50:51 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 20:50:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 20:50:53 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b94ec3f0f3e01d39f7033e85747937598cefb6de79886a6838240a7caa0f681`  
		Last Modified: Fri, 11 Sep 2020 20:51:43 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5006ee3d86dbdcb2110b01e5c30cab655a34754ff1f55d24fd241c8c8046bcc8`  
		Last Modified: Fri, 11 Sep 2020 20:51:52 GMT  
		Size: 35.3 MB (35331410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaeb914a71dcf59c42cf45f0b1e8ae8cedb7dafe092966f06c57ca57f0ea49c6`  
		Last Modified: Fri, 11 Sep 2020 20:51:43 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed51e56effe49113c5b99cbaa51a35e7bb73d979d74f6cfb64432c7f1b6856a2`  
		Last Modified: Fri, 11 Sep 2020 20:51:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ead4b852bd4afca40cbf71ee888422c765f0ad6801a16989f922221ddeccd2`  
		Last Modified: Fri, 11 Sep 2020 20:51:43 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:86fd8acdc9c753435cd47dc999fbbe3d53c6c83f7cb81ea4b8425ac770de5302
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38162728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfab4388bab602ade151776134f0f2e0b2dcf5bf93009298e56f4d8a0146244e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:42:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 22:04:02 GMT
ENV CONSUL_VERSION=1.6.9
# Fri, 11 Sep 2020 22:04:06 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 22:04:24 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 22:04:42 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 22:05:06 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 22:05:30 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 22:05:38 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 22:05:45 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 22:05:54 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 22:05:58 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 22:06:04 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 22:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 22:06:14 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431e303e7f9a61921197b5d7b5a7bca72f8b0e27204dfcdec6e1d5df9dd761e9`  
		Last Modified: Fri, 11 Sep 2020 22:07:33 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8f78930a804ac3b4ff1ca8ff9fe5dfb83ce68d4c5d1aaaafd63ea189831639`  
		Last Modified: Fri, 11 Sep 2020 22:07:41 GMT  
		Size: 35.5 MB (35451464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e660b75be6614d5630fd29c694773652a58a4581d81c46fbbc0085168345eb3`  
		Last Modified: Fri, 11 Sep 2020 22:07:33 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c515443802519bad63dd082309b84c5cdb3d53a83df615a6e247f4973dc207d`  
		Last Modified: Fri, 11 Sep 2020 22:07:33 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9400c6cfba176e2e3293c0f075e9326404e9cc56fb3a91602cf3ea4c930a90ef`  
		Last Modified: Fri, 11 Sep 2020 22:07:33 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; 386

```console
$ docker pull consul@sha256:984ae59d9496401277b91f2c3dff3bf42efb0c7a26ada9eff5caba7eb28b478a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41085837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac1e9ef04be20fe2a661b946e25125c509d53a4efb5328b8661a01fa2c4f82f1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:38:31 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 21:59:40 GMT
ENV CONSUL_VERSION=1.6.9
# Fri, 11 Sep 2020 21:59:41 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 21:59:42 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 21:59:49 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 21:59:50 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 21:59:52 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 21:59:52 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 21:59:52 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 21:59:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 21:59:53 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 21:59:53 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 21:59:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 21:59:54 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87002637186445bf203463d33609d4343260530d55f428ab40141a6291b95333`  
		Last Modified: Fri, 11 Sep 2020 22:00:41 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b563c7f784998b6a756c335329a53ecd7d5038321adca2323a2d947f30f99738`  
		Last Modified: Fri, 11 Sep 2020 22:00:51 GMT  
		Size: 38.3 MB (38290303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3fd34f43bea5324579d611969e48f09a60d267ea118ea7bc7ee33c92644afd8`  
		Last Modified: Fri, 11 Sep 2020 22:00:40 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e949880e1d0d8ee39afe7d49d2e70add21992931fb7b0f0cd4eb12a12873bc9`  
		Last Modified: Fri, 11 Sep 2020 22:00:40 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be241c4a5bc01268746628654901ae6ab9fdaf370d21f55a881e8841752b5469`  
		Last Modified: Fri, 11 Sep 2020 22:00:40 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.6.9`

```console
$ docker pull consul@sha256:574cc0884f2a46336d74a027957d9edff7498fd92562bd26530c734ecc0acf32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.6.9` - linux; amd64

```console
$ docker pull consul@sha256:eddec9d26473fe2e94f4e3bd1b881af9f873dce17f441feaabef2dc531b1b09d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42259611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e74740b420e54b5fabfa7de9085e3f9a92284a068f07e2b2d1ff51da47e8d752`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 21:35:16 GMT
ENV CONSUL_VERSION=1.6.9
# Fri, 11 Sep 2020 21:35:16 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 21:35:17 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 21:35:21 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 21:35:22 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 21:35:23 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 21:35:23 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 21:35:23 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 21:35:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 21:35:23 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 21:35:24 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 21:35:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 21:35:24 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c42497aee15ea85ada3648423d8d60d805b4046840e36e2592010f03b46b5c3`  
		Last Modified: Fri, 11 Sep 2020 21:35:56 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb172b87dfe72a49c6f089cf7da7c050b7da582882d8acf632f5f7912bf3ffa7`  
		Last Modified: Fri, 11 Sep 2020 21:36:01 GMT  
		Size: 39.5 MB (39458832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f80f502d16c7f8614e287d6b921d01d7e0dbd9eb57e6aedaf04567acc00f07`  
		Last Modified: Fri, 11 Sep 2020 21:35:55 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05694da12802199551dded466f04e09ea60449649d97d73f9845a24753edb98d`  
		Last Modified: Fri, 11 Sep 2020 21:35:55 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5013954d81caeedbfde4d469f884e6ec28c3fc8b608b467cd4e34104b573ed6a`  
		Last Modified: Fri, 11 Sep 2020 21:35:55 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6.9` - linux; arm variant v6

```console
$ docker pull consul@sha256:d1b234763bc339b9a12a6b9785ed3e72e65b0a6d605bef8891fa5bcdfc49eba0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37937989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:027d81057134e497189496564bbd4c442b07d593dd9c56234c766a3758974827`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:49:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 20:50:27 GMT
ENV CONSUL_VERSION=1.6.9
# Fri, 11 Sep 2020 20:50:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 20:50:31 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 20:50:40 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 20:50:43 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 20:50:45 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 20:50:46 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 20:50:47 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 20:50:50 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 20:50:51 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 20:50:51 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 20:50:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 20:50:53 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b94ec3f0f3e01d39f7033e85747937598cefb6de79886a6838240a7caa0f681`  
		Last Modified: Fri, 11 Sep 2020 20:51:43 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5006ee3d86dbdcb2110b01e5c30cab655a34754ff1f55d24fd241c8c8046bcc8`  
		Last Modified: Fri, 11 Sep 2020 20:51:52 GMT  
		Size: 35.3 MB (35331410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaeb914a71dcf59c42cf45f0b1e8ae8cedb7dafe092966f06c57ca57f0ea49c6`  
		Last Modified: Fri, 11 Sep 2020 20:51:43 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed51e56effe49113c5b99cbaa51a35e7bb73d979d74f6cfb64432c7f1b6856a2`  
		Last Modified: Fri, 11 Sep 2020 20:51:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ead4b852bd4afca40cbf71ee888422c765f0ad6801a16989f922221ddeccd2`  
		Last Modified: Fri, 11 Sep 2020 20:51:43 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:86fd8acdc9c753435cd47dc999fbbe3d53c6c83f7cb81ea4b8425ac770de5302
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38162728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfab4388bab602ade151776134f0f2e0b2dcf5bf93009298e56f4d8a0146244e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:42:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 22:04:02 GMT
ENV CONSUL_VERSION=1.6.9
# Fri, 11 Sep 2020 22:04:06 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 22:04:24 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 22:04:42 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 22:05:06 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 22:05:30 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 22:05:38 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 22:05:45 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 22:05:54 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 22:05:58 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 22:06:04 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 22:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 22:06:14 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431e303e7f9a61921197b5d7b5a7bca72f8b0e27204dfcdec6e1d5df9dd761e9`  
		Last Modified: Fri, 11 Sep 2020 22:07:33 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8f78930a804ac3b4ff1ca8ff9fe5dfb83ce68d4c5d1aaaafd63ea189831639`  
		Last Modified: Fri, 11 Sep 2020 22:07:41 GMT  
		Size: 35.5 MB (35451464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e660b75be6614d5630fd29c694773652a58a4581d81c46fbbc0085168345eb3`  
		Last Modified: Fri, 11 Sep 2020 22:07:33 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c515443802519bad63dd082309b84c5cdb3d53a83df615a6e247f4973dc207d`  
		Last Modified: Fri, 11 Sep 2020 22:07:33 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9400c6cfba176e2e3293c0f075e9326404e9cc56fb3a91602cf3ea4c930a90ef`  
		Last Modified: Fri, 11 Sep 2020 22:07:33 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6.9` - linux; 386

```console
$ docker pull consul@sha256:984ae59d9496401277b91f2c3dff3bf42efb0c7a26ada9eff5caba7eb28b478a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41085837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac1e9ef04be20fe2a661b946e25125c509d53a4efb5328b8661a01fa2c4f82f1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:38:31 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 21:59:40 GMT
ENV CONSUL_VERSION=1.6.9
# Fri, 11 Sep 2020 21:59:41 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 21:59:42 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 21:59:49 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 21:59:50 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 21:59:52 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 21:59:52 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 21:59:52 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 21:59:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 21:59:53 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 21:59:53 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 21:59:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 21:59:54 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87002637186445bf203463d33609d4343260530d55f428ab40141a6291b95333`  
		Last Modified: Fri, 11 Sep 2020 22:00:41 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b563c7f784998b6a756c335329a53ecd7d5038321adca2323a2d947f30f99738`  
		Last Modified: Fri, 11 Sep 2020 22:00:51 GMT  
		Size: 38.3 MB (38290303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3fd34f43bea5324579d611969e48f09a60d267ea118ea7bc7ee33c92644afd8`  
		Last Modified: Fri, 11 Sep 2020 22:00:40 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e949880e1d0d8ee39afe7d49d2e70add21992931fb7b0f0cd4eb12a12873bc9`  
		Last Modified: Fri, 11 Sep 2020 22:00:40 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be241c4a5bc01268746628654901ae6ab9fdaf370d21f55a881e8841752b5469`  
		Last Modified: Fri, 11 Sep 2020 22:00:40 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7`

```console
$ docker pull consul@sha256:21d27234c57dfb43dc9d425652060ef4a565511d03b263b653e7c5386bb26d24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7` - linux; amd64

```console
$ docker pull consul@sha256:fd06290ad67183ed4f65c35e05efe269dec80b9c665a301ab4e45336dd9b7bf8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.6 MB (43633264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6869b20c1bf31d78cd2525d9607eccb6643ba8ff5aa6ecc5d12fece9e60d5455`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 21:35:04 GMT
ENV CONSUL_VERSION=1.7.8
# Fri, 11 Sep 2020 21:35:04 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 21:35:05 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 21:35:09 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 21:35:10 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 21:35:10 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 21:35:10 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 21:35:11 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 21:35:11 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 21:35:11 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 21:35:11 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 21:35:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 21:35:12 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa86cffd3d009f7a9062b7c62420ed125fec80d5c3ab5c9432246d6b3d7ce11`  
		Last Modified: Fri, 11 Sep 2020 21:35:45 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38e25af134fa51e8e53d03ff4baf1e6b48909de064e5ce2fe617ed73586b48b4`  
		Last Modified: Fri, 11 Sep 2020 21:35:52 GMT  
		Size: 40.8 MB (40832486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8188b0a8b6262076f7dcced96696a6a9f50a6bc10f74abb2dd990a5b9b648e0`  
		Last Modified: Fri, 11 Sep 2020 21:35:46 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c6376cdcf722e41d109f488d4ae9df81f05a1a8fd276f2aa68e2e745048e4f`  
		Last Modified: Fri, 11 Sep 2020 21:35:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b0f8bcd6a04a40bfd629b41a694d2adac2f09fda47e1b93f01f53d8434e3e1`  
		Last Modified: Fri, 11 Sep 2020 21:35:46 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm variant v6

```console
$ docker pull consul@sha256:71cba28e62ec10592039ceb72a8511b55c8f2666b39217047180e9fea9e3de81
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39303513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5e1daef07fc68c15b6937c0599fbd72ada85bb6c790cd7b514ea700a63e59e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:49:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 20:49:56 GMT
ENV CONSUL_VERSION=1.7.8
# Fri, 11 Sep 2020 20:49:56 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 20:49:59 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 20:50:08 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 20:50:11 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 20:50:13 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 20:50:14 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 20:50:15 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 20:50:16 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 20:50:17 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 20:50:17 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 20:50:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 20:50:21 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6844b3063c1a2bd33f1ab8dc40b11e5ea7bff6199f137b4ca0aa498993b51f53`  
		Last Modified: Fri, 11 Sep 2020 20:51:27 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944802fa2b60e84bd8a4d90ab67877d67179e75fe2be2a4c0753a08919a52f50`  
		Last Modified: Fri, 11 Sep 2020 20:51:37 GMT  
		Size: 36.7 MB (36696932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ed00f247e4c41021efcf87e6cbda128e3adc528d414cf7bfba027ead33e923`  
		Last Modified: Fri, 11 Sep 2020 20:51:27 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cb41dbdda2d745c0e2c9997f9824a322e57e9dc601e67264198a27796422ad`  
		Last Modified: Fri, 11 Sep 2020 20:51:27 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377efeb788858a4e3d8de19182644ac7282efa8311db9d1c5d8224880781c8a5`  
		Last Modified: Fri, 11 Sep 2020 20:51:27 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:51c1119b6ec1c5ee48882f16e4c7d210942af9b96b2395d465729c52d9ee5482
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39496036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f3b12a71d518e3edbb1fa3c4122170daddb9edbb227160b17ecd3a90dd82335`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:42:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 22:01:56 GMT
ENV CONSUL_VERSION=1.7.8
# Fri, 11 Sep 2020 22:02:04 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 22:02:26 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 22:02:45 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 22:03:12 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 22:03:25 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 22:03:31 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 22:03:40 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 22:03:44 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 22:03:46 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 22:03:47 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 22:03:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 22:03:49 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a96f60942553a18f38c55b0ca18568571e3621bd8e1ddae3262b07feab1030`  
		Last Modified: Fri, 11 Sep 2020 22:07:10 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e0cd4297ee02a80207a79dc3455964f16d3cb54c2edef6d1c7398a284296e3`  
		Last Modified: Fri, 11 Sep 2020 22:07:18 GMT  
		Size: 36.8 MB (36784771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec9fb361e45c6346c0e5bf642b1fd4906abb07c6bcf01c761b39f9d8a284c86`  
		Last Modified: Fri, 11 Sep 2020 22:07:10 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5565901099d30432fd5ad75a5e4d8d32f3d8a67427fe621ed6c4fa6e7c89b8cf`  
		Last Modified: Fri, 11 Sep 2020 22:07:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b904342259aa54da977754fb2b9bcb5fd3d7ad2d5c2836ef836b506c8bddab7`  
		Last Modified: Fri, 11 Sep 2020 22:07:09 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; 386

```console
$ docker pull consul@sha256:3d3c99aade2e56aec10ad6d175e6f97ac5de7fdfcbf661e9e1195ee6aebe6f35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.4 MB (42408963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ac442a50478849a60eba6ac06de12d7e95150687d984b361c0688db0de6adb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:38:31 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 21:59:21 GMT
ENV CONSUL_VERSION=1.7.8
# Fri, 11 Sep 2020 21:59:21 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 21:59:22 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 21:59:30 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 21:59:31 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 21:59:32 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 21:59:32 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 21:59:33 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 21:59:33 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 21:59:33 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 21:59:34 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 21:59:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 21:59:34 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2d3e0e037cdff5bf18b2976d5e145270da8346bba53257d39053b720133c83`  
		Last Modified: Fri, 11 Sep 2020 22:00:23 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae1c2552334d3caee958b1d6e4824db36891ad942548c972b4d7c1de6d0c0d4`  
		Last Modified: Fri, 11 Sep 2020 22:00:35 GMT  
		Size: 39.6 MB (39613426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f13b1008675439061f393727469a3756faf39cb252a2bedef73c5bc1219d07`  
		Last Modified: Fri, 11 Sep 2020 22:00:24 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12dee0b949df04e806540cc391cd556554a874c76e56019f91521df99e0ea958`  
		Last Modified: Fri, 11 Sep 2020 22:00:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac3b9c6e8f482e955aa02c358187dde38a21b4a89555b0951b0e239c5c7fdff`  
		Last Modified: Fri, 11 Sep 2020 22:00:23 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7.8`

```console
$ docker pull consul@sha256:21d27234c57dfb43dc9d425652060ef4a565511d03b263b653e7c5386bb26d24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7.8` - linux; amd64

```console
$ docker pull consul@sha256:fd06290ad67183ed4f65c35e05efe269dec80b9c665a301ab4e45336dd9b7bf8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.6 MB (43633264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6869b20c1bf31d78cd2525d9607eccb6643ba8ff5aa6ecc5d12fece9e60d5455`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 21:35:04 GMT
ENV CONSUL_VERSION=1.7.8
# Fri, 11 Sep 2020 21:35:04 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 21:35:05 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 21:35:09 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 21:35:10 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 21:35:10 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 21:35:10 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 21:35:11 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 21:35:11 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 21:35:11 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 21:35:11 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 21:35:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 21:35:12 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa86cffd3d009f7a9062b7c62420ed125fec80d5c3ab5c9432246d6b3d7ce11`  
		Last Modified: Fri, 11 Sep 2020 21:35:45 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38e25af134fa51e8e53d03ff4baf1e6b48909de064e5ce2fe617ed73586b48b4`  
		Last Modified: Fri, 11 Sep 2020 21:35:52 GMT  
		Size: 40.8 MB (40832486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8188b0a8b6262076f7dcced96696a6a9f50a6bc10f74abb2dd990a5b9b648e0`  
		Last Modified: Fri, 11 Sep 2020 21:35:46 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c6376cdcf722e41d109f488d4ae9df81f05a1a8fd276f2aa68e2e745048e4f`  
		Last Modified: Fri, 11 Sep 2020 21:35:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b0f8bcd6a04a40bfd629b41a694d2adac2f09fda47e1b93f01f53d8434e3e1`  
		Last Modified: Fri, 11 Sep 2020 21:35:46 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.8` - linux; arm variant v6

```console
$ docker pull consul@sha256:71cba28e62ec10592039ceb72a8511b55c8f2666b39217047180e9fea9e3de81
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39303513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5e1daef07fc68c15b6937c0599fbd72ada85bb6c790cd7b514ea700a63e59e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:49:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 20:49:56 GMT
ENV CONSUL_VERSION=1.7.8
# Fri, 11 Sep 2020 20:49:56 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 20:49:59 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 20:50:08 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 20:50:11 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 20:50:13 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 20:50:14 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 20:50:15 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 20:50:16 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 20:50:17 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 20:50:17 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 20:50:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 20:50:21 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6844b3063c1a2bd33f1ab8dc40b11e5ea7bff6199f137b4ca0aa498993b51f53`  
		Last Modified: Fri, 11 Sep 2020 20:51:27 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944802fa2b60e84bd8a4d90ab67877d67179e75fe2be2a4c0753a08919a52f50`  
		Last Modified: Fri, 11 Sep 2020 20:51:37 GMT  
		Size: 36.7 MB (36696932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ed00f247e4c41021efcf87e6cbda128e3adc528d414cf7bfba027ead33e923`  
		Last Modified: Fri, 11 Sep 2020 20:51:27 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cb41dbdda2d745c0e2c9997f9824a322e57e9dc601e67264198a27796422ad`  
		Last Modified: Fri, 11 Sep 2020 20:51:27 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377efeb788858a4e3d8de19182644ac7282efa8311db9d1c5d8224880781c8a5`  
		Last Modified: Fri, 11 Sep 2020 20:51:27 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:51c1119b6ec1c5ee48882f16e4c7d210942af9b96b2395d465729c52d9ee5482
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39496036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f3b12a71d518e3edbb1fa3c4122170daddb9edbb227160b17ecd3a90dd82335`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:42:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 22:01:56 GMT
ENV CONSUL_VERSION=1.7.8
# Fri, 11 Sep 2020 22:02:04 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 22:02:26 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 22:02:45 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 22:03:12 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 22:03:25 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 22:03:31 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 22:03:40 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 22:03:44 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 22:03:46 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 22:03:47 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 22:03:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 22:03:49 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a96f60942553a18f38c55b0ca18568571e3621bd8e1ddae3262b07feab1030`  
		Last Modified: Fri, 11 Sep 2020 22:07:10 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e0cd4297ee02a80207a79dc3455964f16d3cb54c2edef6d1c7398a284296e3`  
		Last Modified: Fri, 11 Sep 2020 22:07:18 GMT  
		Size: 36.8 MB (36784771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec9fb361e45c6346c0e5bf642b1fd4906abb07c6bcf01c761b39f9d8a284c86`  
		Last Modified: Fri, 11 Sep 2020 22:07:10 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5565901099d30432fd5ad75a5e4d8d32f3d8a67427fe621ed6c4fa6e7c89b8cf`  
		Last Modified: Fri, 11 Sep 2020 22:07:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b904342259aa54da977754fb2b9bcb5fd3d7ad2d5c2836ef836b506c8bddab7`  
		Last Modified: Fri, 11 Sep 2020 22:07:09 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.8` - linux; 386

```console
$ docker pull consul@sha256:3d3c99aade2e56aec10ad6d175e6f97ac5de7fdfcbf661e9e1195ee6aebe6f35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.4 MB (42408963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ac442a50478849a60eba6ac06de12d7e95150687d984b361c0688db0de6adb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:38:31 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 21:59:21 GMT
ENV CONSUL_VERSION=1.7.8
# Fri, 11 Sep 2020 21:59:21 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 21:59:22 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 21:59:30 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 21:59:31 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 21:59:32 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 21:59:32 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 21:59:33 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 21:59:33 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 21:59:33 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 21:59:34 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 21:59:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 21:59:34 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2d3e0e037cdff5bf18b2976d5e145270da8346bba53257d39053b720133c83`  
		Last Modified: Fri, 11 Sep 2020 22:00:23 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae1c2552334d3caee958b1d6e4824db36891ad942548c972b4d7c1de6d0c0d4`  
		Last Modified: Fri, 11 Sep 2020 22:00:35 GMT  
		Size: 39.6 MB (39613426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f13b1008675439061f393727469a3756faf39cb252a2bedef73c5bc1219d07`  
		Last Modified: Fri, 11 Sep 2020 22:00:24 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12dee0b949df04e806540cc391cd556554a874c76e56019f91521df99e0ea958`  
		Last Modified: Fri, 11 Sep 2020 22:00:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac3b9c6e8f482e955aa02c358187dde38a21b4a89555b0951b0e239c5c7fdff`  
		Last Modified: Fri, 11 Sep 2020 22:00:23 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8`

```console
$ docker pull consul@sha256:36fd1f8ca4d702c7dce0d58662893245ff417c863ba38226e73be7f722d0efcb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8` - linux; amd64

```console
$ docker pull consul@sha256:e9b4eca3141960e18f2c09d1dcc5e1232ddc8d3bc077b5577460b4d3ee96a7ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46719494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3945f796958277e335d0fc06f16ccf59b2ffe67b1550e820bfae255cd0e02362`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 21:34:51 GMT
ENV CONSUL_VERSION=1.8.4
# Fri, 11 Sep 2020 21:34:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 21:34:52 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 21:34:56 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 21:34:57 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 21:34:58 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 21:34:58 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 21:34:58 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 21:34:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 21:34:59 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 21:34:59 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 21:34:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 21:34:59 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f53b97be57a8b151b90aec8c0bae62ff8fdc031c1f1e6b4aa5b2f89fbde0b0`  
		Last Modified: Fri, 11 Sep 2020 21:35:32 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc3ccb924c034d384494391649d39785a32803293fa81ab720bcea287a190ec`  
		Last Modified: Fri, 11 Sep 2020 21:35:40 GMT  
		Size: 43.9 MB (43918715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d16d05c330fa3bcea904ee0349c9181bc61c774f7cd5f9e5b2f2c09f36c7c5e`  
		Last Modified: Fri, 11 Sep 2020 21:35:32 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ed495875d84a63a5b86b2b9bb50739a6f2c4c2847882bfc7b39fc40171f2f3`  
		Last Modified: Fri, 11 Sep 2020 21:35:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c418676c3be3c8a9a79211b1318c090eab2b0ff1bbc0cff682107f32b4c85f96`  
		Last Modified: Fri, 11 Sep 2020 21:35:32 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm variant v6

```console
$ docker pull consul@sha256:aafaaf0a09da25bd0cb54bee1602b40cc1f7ef193138e4f6b434f76a943c0fe2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41989701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a43a86100da6105b536645f761c3b8ddceb32dcd97aa0640f33164a622dfe57e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:49:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 20:49:29 GMT
ENV CONSUL_VERSION=1.8.4
# Fri, 11 Sep 2020 20:49:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 20:49:31 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 20:49:40 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 20:49:44 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 20:49:46 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 20:49:46 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 20:49:47 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 20:49:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 20:49:48 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 20:49:48 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 20:49:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 20:49:50 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d7d80d413d641bef620f785978bda397aeadb9d40c19888f1988f929a889be`  
		Last Modified: Fri, 11 Sep 2020 20:51:09 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132a3b58482ee0d780b5c237f45cfd9e340608f0251760e4da695f7c9c61f9e2`  
		Last Modified: Fri, 11 Sep 2020 20:51:19 GMT  
		Size: 39.4 MB (39383119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7fc35438c3d463979d24a583bf530ce2f1d0577a22458d98d4101f6744f809`  
		Last Modified: Fri, 11 Sep 2020 20:51:08 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87522bb599e02c975c75cc6765f06913218b8a993a2af1c128f6c539df64d6d0`  
		Last Modified: Fri, 11 Sep 2020 20:51:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59c8f2ab204e55afa3d65f24e4a8faddc5a897301d01f6eb835b1dd22b89510`  
		Last Modified: Fri, 11 Sep 2020 20:51:08 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:a40032447c01d9199321d883d42bbbe28bd2edce3c24b5eef21ac4e9974fe91c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.2 MB (42167940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86404cb901315a0cf904b7bc3764adc5f5694b74c4be6dc955b8a946cd897449`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:42:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 22:00:24 GMT
ENV CONSUL_VERSION=1.8.4
# Fri, 11 Sep 2020 22:00:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 22:00:50 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 22:01:02 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 22:01:05 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 22:01:07 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 22:01:08 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 22:01:08 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 22:01:12 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 22:01:17 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 22:01:18 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 22:01:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 22:01:34 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967b89682f403f9f025fc8454190c0f8e8162fc4183780106bd9a03e6c5ce3bf`  
		Last Modified: Fri, 11 Sep 2020 22:06:40 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cb574a495d472489845a8f9dfdeddb588f938b01a34301a6ac8c68bcfa42e8`  
		Last Modified: Fri, 11 Sep 2020 22:06:56 GMT  
		Size: 39.5 MB (39456676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc26476c498ce9296f247e0ecac25472ee44d392d4b28756f5a620f51c590257`  
		Last Modified: Fri, 11 Sep 2020 22:06:40 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1722096cd9b723886ac571b7557ff3ebe32219e8bf49c93ea8065fd1c9254fd`  
		Last Modified: Fri, 11 Sep 2020 22:06:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da60306d6f2cdacb33e2aa91924687a0f8bc40bada23a1fc8d24fc2d5e787cff`  
		Last Modified: Fri, 11 Sep 2020 22:06:40 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; 386

```console
$ docker pull consul@sha256:fe88187e063fa98c7b83bb5094c1df899a9003e92c8b582e6641d7c7f27d106c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46231133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe596555cb13dc116b245bfeaaa59d15b587e674ce89dcf752c5016a4adbdda5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:38:31 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 21:59:02 GMT
ENV CONSUL_VERSION=1.8.4
# Fri, 11 Sep 2020 21:59:02 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 21:59:03 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 21:59:11 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 21:59:12 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 21:59:13 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 21:59:14 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 21:59:14 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 21:59:14 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 21:59:14 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 21:59:15 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 21:59:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 21:59:15 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad59a362419a53b3483c2f21b4c3df30b6eb9580bc9f609a35a6288dd3d7680`  
		Last Modified: Fri, 11 Sep 2020 22:00:06 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f5fa59eaf9c3a165c60327e6d25d89b4a35e355fd51476f0177e3e8f4f11a6`  
		Last Modified: Fri, 11 Sep 2020 22:00:19 GMT  
		Size: 43.4 MB (43435597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2794fb4df6e993c680707c30f894a3ac91561702c42c31ae356eec1f953525e`  
		Last Modified: Fri, 11 Sep 2020 22:00:06 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4370526947ff161df38592e4692c198fd3bf20a5719c02a69a0f987d9f1db10f`  
		Last Modified: Fri, 11 Sep 2020 22:00:06 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76afc73ed62aead0205076b3431c1d781c03dcc4c164ff655398b40c8cadece2`  
		Last Modified: Fri, 11 Sep 2020 22:00:06 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8.4`

```console
$ docker pull consul@sha256:36fd1f8ca4d702c7dce0d58662893245ff417c863ba38226e73be7f722d0efcb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8.4` - linux; amd64

```console
$ docker pull consul@sha256:e9b4eca3141960e18f2c09d1dcc5e1232ddc8d3bc077b5577460b4d3ee96a7ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46719494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3945f796958277e335d0fc06f16ccf59b2ffe67b1550e820bfae255cd0e02362`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 21:34:51 GMT
ENV CONSUL_VERSION=1.8.4
# Fri, 11 Sep 2020 21:34:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 21:34:52 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 21:34:56 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 21:34:57 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 21:34:58 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 21:34:58 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 21:34:58 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 21:34:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 21:34:59 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 21:34:59 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 21:34:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 21:34:59 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f53b97be57a8b151b90aec8c0bae62ff8fdc031c1f1e6b4aa5b2f89fbde0b0`  
		Last Modified: Fri, 11 Sep 2020 21:35:32 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc3ccb924c034d384494391649d39785a32803293fa81ab720bcea287a190ec`  
		Last Modified: Fri, 11 Sep 2020 21:35:40 GMT  
		Size: 43.9 MB (43918715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d16d05c330fa3bcea904ee0349c9181bc61c774f7cd5f9e5b2f2c09f36c7c5e`  
		Last Modified: Fri, 11 Sep 2020 21:35:32 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ed495875d84a63a5b86b2b9bb50739a6f2c4c2847882bfc7b39fc40171f2f3`  
		Last Modified: Fri, 11 Sep 2020 21:35:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c418676c3be3c8a9a79211b1318c090eab2b0ff1bbc0cff682107f32b4c85f96`  
		Last Modified: Fri, 11 Sep 2020 21:35:32 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.4` - linux; arm variant v6

```console
$ docker pull consul@sha256:aafaaf0a09da25bd0cb54bee1602b40cc1f7ef193138e4f6b434f76a943c0fe2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41989701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a43a86100da6105b536645f761c3b8ddceb32dcd97aa0640f33164a622dfe57e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:49:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 20:49:29 GMT
ENV CONSUL_VERSION=1.8.4
# Fri, 11 Sep 2020 20:49:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 20:49:31 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 20:49:40 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 20:49:44 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 20:49:46 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 20:49:46 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 20:49:47 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 20:49:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 20:49:48 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 20:49:48 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 20:49:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 20:49:50 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d7d80d413d641bef620f785978bda397aeadb9d40c19888f1988f929a889be`  
		Last Modified: Fri, 11 Sep 2020 20:51:09 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132a3b58482ee0d780b5c237f45cfd9e340608f0251760e4da695f7c9c61f9e2`  
		Last Modified: Fri, 11 Sep 2020 20:51:19 GMT  
		Size: 39.4 MB (39383119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7fc35438c3d463979d24a583bf530ce2f1d0577a22458d98d4101f6744f809`  
		Last Modified: Fri, 11 Sep 2020 20:51:08 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87522bb599e02c975c75cc6765f06913218b8a993a2af1c128f6c539df64d6d0`  
		Last Modified: Fri, 11 Sep 2020 20:51:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59c8f2ab204e55afa3d65f24e4a8faddc5a897301d01f6eb835b1dd22b89510`  
		Last Modified: Fri, 11 Sep 2020 20:51:08 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.4` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:a40032447c01d9199321d883d42bbbe28bd2edce3c24b5eef21ac4e9974fe91c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.2 MB (42167940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86404cb901315a0cf904b7bc3764adc5f5694b74c4be6dc955b8a946cd897449`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:42:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 22:00:24 GMT
ENV CONSUL_VERSION=1.8.4
# Fri, 11 Sep 2020 22:00:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 22:00:50 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 22:01:02 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 22:01:05 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 22:01:07 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 22:01:08 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 22:01:08 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 22:01:12 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 22:01:17 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 22:01:18 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 22:01:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 22:01:34 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967b89682f403f9f025fc8454190c0f8e8162fc4183780106bd9a03e6c5ce3bf`  
		Last Modified: Fri, 11 Sep 2020 22:06:40 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cb574a495d472489845a8f9dfdeddb588f938b01a34301a6ac8c68bcfa42e8`  
		Last Modified: Fri, 11 Sep 2020 22:06:56 GMT  
		Size: 39.5 MB (39456676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc26476c498ce9296f247e0ecac25472ee44d392d4b28756f5a620f51c590257`  
		Last Modified: Fri, 11 Sep 2020 22:06:40 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1722096cd9b723886ac571b7557ff3ebe32219e8bf49c93ea8065fd1c9254fd`  
		Last Modified: Fri, 11 Sep 2020 22:06:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da60306d6f2cdacb33e2aa91924687a0f8bc40bada23a1fc8d24fc2d5e787cff`  
		Last Modified: Fri, 11 Sep 2020 22:06:40 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.4` - linux; 386

```console
$ docker pull consul@sha256:fe88187e063fa98c7b83bb5094c1df899a9003e92c8b582e6641d7c7f27d106c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46231133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe596555cb13dc116b245bfeaaa59d15b587e674ce89dcf752c5016a4adbdda5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:38:31 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 21:59:02 GMT
ENV CONSUL_VERSION=1.8.4
# Fri, 11 Sep 2020 21:59:02 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 21:59:03 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 21:59:11 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 21:59:12 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 21:59:13 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 21:59:14 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 21:59:14 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 21:59:14 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 21:59:14 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 21:59:15 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 21:59:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 21:59:15 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad59a362419a53b3483c2f21b4c3df30b6eb9580bc9f609a35a6288dd3d7680`  
		Last Modified: Fri, 11 Sep 2020 22:00:06 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f5fa59eaf9c3a165c60327e6d25d89b4a35e355fd51476f0177e3e8f4f11a6`  
		Last Modified: Fri, 11 Sep 2020 22:00:19 GMT  
		Size: 43.4 MB (43435597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2794fb4df6e993c680707c30f894a3ac91561702c42c31ae356eec1f953525e`  
		Last Modified: Fri, 11 Sep 2020 22:00:06 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4370526947ff161df38592e4692c198fd3bf20a5719c02a69a0f987d9f1db10f`  
		Last Modified: Fri, 11 Sep 2020 22:00:06 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76afc73ed62aead0205076b3431c1d781c03dcc4c164ff655398b40c8cadece2`  
		Last Modified: Fri, 11 Sep 2020 22:00:06 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9.0-beta`

```console
$ docker pull consul@sha256:fbb99a0c59bd45d0724532ae8a1e2b50458becf2c9f75170a257336d72ea64c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9.0-beta` - linux; amd64

```console
$ docker pull consul@sha256:93beed4c1164b3ea24799046c4be26d3e8bf4e5ff727fb3fde974c149824265a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (47994383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:964d692fbce612e9e67a567be57bcb9859d0a0278375e93dfb4da70147842801`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 12 Oct 2020 22:22:15 GMT
ENV CONSUL_VERSION=1.9.0-beta1
# Mon, 12 Oct 2020 22:22:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 12 Oct 2020 22:22:16 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 12 Oct 2020 22:22:21 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 12 Oct 2020 22:22:21 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 12 Oct 2020 22:22:22 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 12 Oct 2020 22:22:22 GMT
VOLUME [/consul/data]
# Mon, 12 Oct 2020 22:22:22 GMT
EXPOSE 8300
# Mon, 12 Oct 2020 22:22:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 12 Oct 2020 22:22:23 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 12 Oct 2020 22:22:23 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 12 Oct 2020 22:22:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Oct 2020 22:22:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3017652a3d3658694bb2a2bb454b5fa6455549d6453beced201949d72a23bfe5`  
		Last Modified: Mon, 12 Oct 2020 22:22:42 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b151ef90caabd14c7236bbf180a8b6df6df9487d87d10affbd8a9972e63db96`  
		Last Modified: Mon, 12 Oct 2020 22:23:14 GMT  
		Size: 45.2 MB (45193611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc5f1955835928aa40afef11414617267f87fd99dcef5b556f6160eab495728`  
		Last Modified: Mon, 12 Oct 2020 22:22:42 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d067c492a0b8f26e8ff71a3ff2398c713059def8fac5358e58a858bacaaa88d`  
		Last Modified: Mon, 12 Oct 2020 22:22:42 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee1fc1229b9953b6020dfaac75a9d3cfb4520118149eae1b273d9af6c8038dd`  
		Last Modified: Mon, 12 Oct 2020 22:22:42 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.0-beta` - linux; arm variant v6

```console
$ docker pull consul@sha256:348a563982eaf5c9ae00ee0fb70d3ff4bcd1ec12af33deda37d69325738d8ad4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43134535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f5e3b61f8932a36ed8acb0f5834a69536e2fff8982d4f2440522047a66e929c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:49:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 12 Oct 2020 22:50:36 GMT
ENV CONSUL_VERSION=1.9.0-beta1
# Mon, 12 Oct 2020 22:50:37 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 12 Oct 2020 22:50:43 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 12 Oct 2020 22:51:00 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 12 Oct 2020 22:51:08 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 12 Oct 2020 22:51:15 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 12 Oct 2020 22:51:16 GMT
VOLUME [/consul/data]
# Mon, 12 Oct 2020 22:51:17 GMT
EXPOSE 8300
# Mon, 12 Oct 2020 22:51:18 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 12 Oct 2020 22:51:20 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 12 Oct 2020 22:51:21 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 12 Oct 2020 22:51:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Oct 2020 22:51:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baae847a49ee218ec06142c4065e79a6a3d9a57e9bad1a78b0a3aef8a8f821d`  
		Last Modified: Mon, 12 Oct 2020 22:51:54 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab14305e5ad8d47865a81f4e744ec17905761de68caf2ed527c2449db568cf4`  
		Last Modified: Mon, 12 Oct 2020 22:52:07 GMT  
		Size: 40.5 MB (40527952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769d3049cd74a6d4b0bc6b2869b0290493fb0c0154dd4f0acb48e763f9042fff`  
		Last Modified: Mon, 12 Oct 2020 22:51:54 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c661ca0bee31ff3873bb35eccfc942d750ca2ab11e78bd6b1e22f7581b9d5bf6`  
		Last Modified: Mon, 12 Oct 2020 22:51:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1348b6ecd9609ad137e55e3e065eff3a7cacc4a23ce87fba048e6276e232147e`  
		Last Modified: Mon, 12 Oct 2020 22:51:55 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.0-beta` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:f01e4dcfdbeea8bef80c73de5e526f43cd706c1cfb6e04da4e902e958341df06
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.3 MB (43320192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3686993d5e5092bd32e8d2ce30bac8c9c43b2ad06423e063968404a794ca6156`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:42:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 12 Oct 2020 23:14:17 GMT
ENV CONSUL_VERSION=1.9.0-beta1
# Mon, 12 Oct 2020 23:14:19 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 12 Oct 2020 23:14:24 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 12 Oct 2020 23:14:36 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 12 Oct 2020 23:14:40 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 12 Oct 2020 23:14:44 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 12 Oct 2020 23:14:46 GMT
VOLUME [/consul/data]
# Mon, 12 Oct 2020 23:14:47 GMT
EXPOSE 8300
# Mon, 12 Oct 2020 23:14:48 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 12 Oct 2020 23:14:50 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 12 Oct 2020 23:14:51 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 12 Oct 2020 23:14:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Oct 2020 23:14:52 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614a8e0f82d4a1fe6beafbf3048fd50bc1023cca12950c987f7872005df0f327`  
		Last Modified: Mon, 12 Oct 2020 23:15:26 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b827bc52126edbae7e007058d6c929312ee1aa3f6fc2329c38ca907a7e3e18d6`  
		Last Modified: Mon, 12 Oct 2020 23:15:39 GMT  
		Size: 40.6 MB (40608930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3a7539e24bbb1d754619c38ac90472d61e2af15b56244499ef95d20dad91a3`  
		Last Modified: Mon, 12 Oct 2020 23:15:26 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d8c054b779d9220d2af763a84b0fcdfe9e8cf885e30886cfc1f7208ab561db`  
		Last Modified: Mon, 12 Oct 2020 23:15:26 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837f38d140259e4128f5a23efee50375697b511ae664c63128cc564c12272669`  
		Last Modified: Mon, 12 Oct 2020 23:15:26 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.0-beta` - linux; 386

```console
$ docker pull consul@sha256:da9148ca248986b2f1b0aa7da51b1860a531fb781dcc3bd4817985873b2f8f33
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.5 MB (47513955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:959f6812f70d07344c4b3e5a06dbfbc9e4df77a9919d34af3266947c2cc284ac`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:38:31 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 12 Oct 2020 22:38:24 GMT
ENV CONSUL_VERSION=1.9.0-beta1
# Mon, 12 Oct 2020 22:38:25 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 12 Oct 2020 22:38:25 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 12 Oct 2020 22:38:32 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 12 Oct 2020 22:38:33 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 12 Oct 2020 22:38:34 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 12 Oct 2020 22:38:34 GMT
VOLUME [/consul/data]
# Mon, 12 Oct 2020 22:38:34 GMT
EXPOSE 8300
# Mon, 12 Oct 2020 22:38:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 12 Oct 2020 22:38:35 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 12 Oct 2020 22:38:35 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 12 Oct 2020 22:38:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Oct 2020 22:38:36 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ddf8b9267f3c2f4646bcbb77ecde6e4f8a34c9d08658fa663f1c0f3a83a2b8`  
		Last Modified: Mon, 12 Oct 2020 22:38:57 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc13bca9b57224b92b79966a934c742456d8af4a76d561672de473aa37a7d9e`  
		Last Modified: Mon, 12 Oct 2020 22:39:08 GMT  
		Size: 44.7 MB (44718423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd2b6c9cc72e98506c0e117f24ba8e1d780cc2a38e4c64d16389dae82135a5c0`  
		Last Modified: Mon, 12 Oct 2020 22:38:58 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75820e80e22edce1f7ecc0cf91af07c3a6e47cc325ed420d679d8b0fb015e8c`  
		Last Modified: Mon, 12 Oct 2020 22:38:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c81f531f29e02efa7a46794e5a824ae9f39f83aa0b20b9a13a1865b197511da`  
		Last Modified: Mon, 12 Oct 2020 22:38:57 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9.0-beta1`

```console
$ docker pull consul@sha256:fbb99a0c59bd45d0724532ae8a1e2b50458becf2c9f75170a257336d72ea64c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9.0-beta1` - linux; amd64

```console
$ docker pull consul@sha256:93beed4c1164b3ea24799046c4be26d3e8bf4e5ff727fb3fde974c149824265a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (47994383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:964d692fbce612e9e67a567be57bcb9859d0a0278375e93dfb4da70147842801`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 12 Oct 2020 22:22:15 GMT
ENV CONSUL_VERSION=1.9.0-beta1
# Mon, 12 Oct 2020 22:22:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 12 Oct 2020 22:22:16 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 12 Oct 2020 22:22:21 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 12 Oct 2020 22:22:21 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 12 Oct 2020 22:22:22 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 12 Oct 2020 22:22:22 GMT
VOLUME [/consul/data]
# Mon, 12 Oct 2020 22:22:22 GMT
EXPOSE 8300
# Mon, 12 Oct 2020 22:22:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 12 Oct 2020 22:22:23 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 12 Oct 2020 22:22:23 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 12 Oct 2020 22:22:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Oct 2020 22:22:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3017652a3d3658694bb2a2bb454b5fa6455549d6453beced201949d72a23bfe5`  
		Last Modified: Mon, 12 Oct 2020 22:22:42 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b151ef90caabd14c7236bbf180a8b6df6df9487d87d10affbd8a9972e63db96`  
		Last Modified: Mon, 12 Oct 2020 22:23:14 GMT  
		Size: 45.2 MB (45193611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc5f1955835928aa40afef11414617267f87fd99dcef5b556f6160eab495728`  
		Last Modified: Mon, 12 Oct 2020 22:22:42 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d067c492a0b8f26e8ff71a3ff2398c713059def8fac5358e58a858bacaaa88d`  
		Last Modified: Mon, 12 Oct 2020 22:22:42 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee1fc1229b9953b6020dfaac75a9d3cfb4520118149eae1b273d9af6c8038dd`  
		Last Modified: Mon, 12 Oct 2020 22:22:42 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.0-beta1` - linux; arm variant v6

```console
$ docker pull consul@sha256:348a563982eaf5c9ae00ee0fb70d3ff4bcd1ec12af33deda37d69325738d8ad4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43134535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f5e3b61f8932a36ed8acb0f5834a69536e2fff8982d4f2440522047a66e929c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:49:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 12 Oct 2020 22:50:36 GMT
ENV CONSUL_VERSION=1.9.0-beta1
# Mon, 12 Oct 2020 22:50:37 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 12 Oct 2020 22:50:43 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 12 Oct 2020 22:51:00 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 12 Oct 2020 22:51:08 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 12 Oct 2020 22:51:15 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 12 Oct 2020 22:51:16 GMT
VOLUME [/consul/data]
# Mon, 12 Oct 2020 22:51:17 GMT
EXPOSE 8300
# Mon, 12 Oct 2020 22:51:18 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 12 Oct 2020 22:51:20 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 12 Oct 2020 22:51:21 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 12 Oct 2020 22:51:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Oct 2020 22:51:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baae847a49ee218ec06142c4065e79a6a3d9a57e9bad1a78b0a3aef8a8f821d`  
		Last Modified: Mon, 12 Oct 2020 22:51:54 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab14305e5ad8d47865a81f4e744ec17905761de68caf2ed527c2449db568cf4`  
		Last Modified: Mon, 12 Oct 2020 22:52:07 GMT  
		Size: 40.5 MB (40527952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769d3049cd74a6d4b0bc6b2869b0290493fb0c0154dd4f0acb48e763f9042fff`  
		Last Modified: Mon, 12 Oct 2020 22:51:54 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c661ca0bee31ff3873bb35eccfc942d750ca2ab11e78bd6b1e22f7581b9d5bf6`  
		Last Modified: Mon, 12 Oct 2020 22:51:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1348b6ecd9609ad137e55e3e065eff3a7cacc4a23ce87fba048e6276e232147e`  
		Last Modified: Mon, 12 Oct 2020 22:51:55 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.0-beta1` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:f01e4dcfdbeea8bef80c73de5e526f43cd706c1cfb6e04da4e902e958341df06
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.3 MB (43320192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3686993d5e5092bd32e8d2ce30bac8c9c43b2ad06423e063968404a794ca6156`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:42:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 12 Oct 2020 23:14:17 GMT
ENV CONSUL_VERSION=1.9.0-beta1
# Mon, 12 Oct 2020 23:14:19 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 12 Oct 2020 23:14:24 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 12 Oct 2020 23:14:36 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 12 Oct 2020 23:14:40 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 12 Oct 2020 23:14:44 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 12 Oct 2020 23:14:46 GMT
VOLUME [/consul/data]
# Mon, 12 Oct 2020 23:14:47 GMT
EXPOSE 8300
# Mon, 12 Oct 2020 23:14:48 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 12 Oct 2020 23:14:50 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 12 Oct 2020 23:14:51 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 12 Oct 2020 23:14:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Oct 2020 23:14:52 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614a8e0f82d4a1fe6beafbf3048fd50bc1023cca12950c987f7872005df0f327`  
		Last Modified: Mon, 12 Oct 2020 23:15:26 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b827bc52126edbae7e007058d6c929312ee1aa3f6fc2329c38ca907a7e3e18d6`  
		Last Modified: Mon, 12 Oct 2020 23:15:39 GMT  
		Size: 40.6 MB (40608930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3a7539e24bbb1d754619c38ac90472d61e2af15b56244499ef95d20dad91a3`  
		Last Modified: Mon, 12 Oct 2020 23:15:26 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d8c054b779d9220d2af763a84b0fcdfe9e8cf885e30886cfc1f7208ab561db`  
		Last Modified: Mon, 12 Oct 2020 23:15:26 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837f38d140259e4128f5a23efee50375697b511ae664c63128cc564c12272669`  
		Last Modified: Mon, 12 Oct 2020 23:15:26 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.0-beta1` - linux; 386

```console
$ docker pull consul@sha256:da9148ca248986b2f1b0aa7da51b1860a531fb781dcc3bd4817985873b2f8f33
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.5 MB (47513955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:959f6812f70d07344c4b3e5a06dbfbc9e4df77a9919d34af3266947c2cc284ac`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:38:31 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 12 Oct 2020 22:38:24 GMT
ENV CONSUL_VERSION=1.9.0-beta1
# Mon, 12 Oct 2020 22:38:25 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 12 Oct 2020 22:38:25 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 12 Oct 2020 22:38:32 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 12 Oct 2020 22:38:33 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 12 Oct 2020 22:38:34 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 12 Oct 2020 22:38:34 GMT
VOLUME [/consul/data]
# Mon, 12 Oct 2020 22:38:34 GMT
EXPOSE 8300
# Mon, 12 Oct 2020 22:38:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 12 Oct 2020 22:38:35 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 12 Oct 2020 22:38:35 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 12 Oct 2020 22:38:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Oct 2020 22:38:36 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ddf8b9267f3c2f4646bcbb77ecde6e4f8a34c9d08658fa663f1c0f3a83a2b8`  
		Last Modified: Mon, 12 Oct 2020 22:38:57 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc13bca9b57224b92b79966a934c742456d8af4a76d561672de473aa37a7d9e`  
		Last Modified: Mon, 12 Oct 2020 22:39:08 GMT  
		Size: 44.7 MB (44718423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd2b6c9cc72e98506c0e117f24ba8e1d780cc2a38e4c64d16389dae82135a5c0`  
		Last Modified: Mon, 12 Oct 2020 22:38:58 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75820e80e22edce1f7ecc0cf91af07c3a6e47cc325ed420d679d8b0fb015e8c`  
		Last Modified: Mon, 12 Oct 2020 22:38:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c81f531f29e02efa7a46794e5a824ae9f39f83aa0b20b9a13a1865b197511da`  
		Last Modified: Mon, 12 Oct 2020 22:38:57 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:36fd1f8ca4d702c7dce0d58662893245ff417c863ba38226e73be7f722d0efcb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:e9b4eca3141960e18f2c09d1dcc5e1232ddc8d3bc077b5577460b4d3ee96a7ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46719494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3945f796958277e335d0fc06f16ccf59b2ffe67b1550e820bfae255cd0e02362`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 21:34:51 GMT
ENV CONSUL_VERSION=1.8.4
# Fri, 11 Sep 2020 21:34:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 21:34:52 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 21:34:56 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 21:34:57 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 21:34:58 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 21:34:58 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 21:34:58 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 21:34:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 21:34:59 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 21:34:59 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 21:34:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 21:34:59 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f53b97be57a8b151b90aec8c0bae62ff8fdc031c1f1e6b4aa5b2f89fbde0b0`  
		Last Modified: Fri, 11 Sep 2020 21:35:32 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc3ccb924c034d384494391649d39785a32803293fa81ab720bcea287a190ec`  
		Last Modified: Fri, 11 Sep 2020 21:35:40 GMT  
		Size: 43.9 MB (43918715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d16d05c330fa3bcea904ee0349c9181bc61c774f7cd5f9e5b2f2c09f36c7c5e`  
		Last Modified: Fri, 11 Sep 2020 21:35:32 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ed495875d84a63a5b86b2b9bb50739a6f2c4c2847882bfc7b39fc40171f2f3`  
		Last Modified: Fri, 11 Sep 2020 21:35:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c418676c3be3c8a9a79211b1318c090eab2b0ff1bbc0cff682107f32b4c85f96`  
		Last Modified: Fri, 11 Sep 2020 21:35:32 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:aafaaf0a09da25bd0cb54bee1602b40cc1f7ef193138e4f6b434f76a943c0fe2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41989701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a43a86100da6105b536645f761c3b8ddceb32dcd97aa0640f33164a622dfe57e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:49:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 20:49:29 GMT
ENV CONSUL_VERSION=1.8.4
# Fri, 11 Sep 2020 20:49:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 20:49:31 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 20:49:40 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 20:49:44 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 20:49:46 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 20:49:46 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 20:49:47 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 20:49:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 20:49:48 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 20:49:48 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 20:49:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 20:49:50 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d7d80d413d641bef620f785978bda397aeadb9d40c19888f1988f929a889be`  
		Last Modified: Fri, 11 Sep 2020 20:51:09 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132a3b58482ee0d780b5c237f45cfd9e340608f0251760e4da695f7c9c61f9e2`  
		Last Modified: Fri, 11 Sep 2020 20:51:19 GMT  
		Size: 39.4 MB (39383119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7fc35438c3d463979d24a583bf530ce2f1d0577a22458d98d4101f6744f809`  
		Last Modified: Fri, 11 Sep 2020 20:51:08 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87522bb599e02c975c75cc6765f06913218b8a993a2af1c128f6c539df64d6d0`  
		Last Modified: Fri, 11 Sep 2020 20:51:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59c8f2ab204e55afa3d65f24e4a8faddc5a897301d01f6eb835b1dd22b89510`  
		Last Modified: Fri, 11 Sep 2020 20:51:08 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:a40032447c01d9199321d883d42bbbe28bd2edce3c24b5eef21ac4e9974fe91c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.2 MB (42167940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86404cb901315a0cf904b7bc3764adc5f5694b74c4be6dc955b8a946cd897449`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:42:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 22:00:24 GMT
ENV CONSUL_VERSION=1.8.4
# Fri, 11 Sep 2020 22:00:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 22:00:50 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 22:01:02 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 22:01:05 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 22:01:07 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 22:01:08 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 22:01:08 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 22:01:12 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 22:01:17 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 22:01:18 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 22:01:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 22:01:34 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967b89682f403f9f025fc8454190c0f8e8162fc4183780106bd9a03e6c5ce3bf`  
		Last Modified: Fri, 11 Sep 2020 22:06:40 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cb574a495d472489845a8f9dfdeddb588f938b01a34301a6ac8c68bcfa42e8`  
		Last Modified: Fri, 11 Sep 2020 22:06:56 GMT  
		Size: 39.5 MB (39456676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc26476c498ce9296f247e0ecac25472ee44d392d4b28756f5a620f51c590257`  
		Last Modified: Fri, 11 Sep 2020 22:06:40 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1722096cd9b723886ac571b7557ff3ebe32219e8bf49c93ea8065fd1c9254fd`  
		Last Modified: Fri, 11 Sep 2020 22:06:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da60306d6f2cdacb33e2aa91924687a0f8bc40bada23a1fc8d24fc2d5e787cff`  
		Last Modified: Fri, 11 Sep 2020 22:06:40 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:fe88187e063fa98c7b83bb5094c1df899a9003e92c8b582e6641d7c7f27d106c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46231133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe596555cb13dc116b245bfeaaa59d15b587e674ce89dcf752c5016a4adbdda5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:38:31 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 21:59:02 GMT
ENV CONSUL_VERSION=1.8.4
# Fri, 11 Sep 2020 21:59:02 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 21:59:03 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 21:59:11 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 21:59:12 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 21:59:13 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 21:59:14 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 21:59:14 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 21:59:14 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 21:59:14 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 21:59:15 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 21:59:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 21:59:15 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad59a362419a53b3483c2f21b4c3df30b6eb9580bc9f609a35a6288dd3d7680`  
		Last Modified: Fri, 11 Sep 2020 22:00:06 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f5fa59eaf9c3a165c60327e6d25d89b4a35e355fd51476f0177e3e8f4f11a6`  
		Last Modified: Fri, 11 Sep 2020 22:00:19 GMT  
		Size: 43.4 MB (43435597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2794fb4df6e993c680707c30f894a3ac91561702c42c31ae356eec1f953525e`  
		Last Modified: Fri, 11 Sep 2020 22:00:06 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4370526947ff161df38592e4692c198fd3bf20a5719c02a69a0f987d9f1db10f`  
		Last Modified: Fri, 11 Sep 2020 22:00:06 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76afc73ed62aead0205076b3431c1d781c03dcc4c164ff655398b40c8cadece2`  
		Last Modified: Fri, 11 Sep 2020 22:00:06 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
