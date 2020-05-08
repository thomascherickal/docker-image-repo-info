<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:0.9`](#consul09)
-	[`consul:0.9.4`](#consul094)
-	[`consul:1.0`](#consul10)
-	[`consul:1.0.8`](#consul108)
-	[`consul:1.1`](#consul11)
-	[`consul:1.1.1`](#consul111)
-	[`consul:1.2`](#consul12)
-	[`consul:1.2.4`](#consul124)
-	[`consul:1.3`](#consul13)
-	[`consul:1.3.1`](#consul131)
-	[`consul:1.4`](#consul14)
-	[`consul:1.4.5`](#consul145)
-	[`consul:1.5`](#consul15)
-	[`consul:1.5.3`](#consul153)
-	[`consul:1.6`](#consul16)
-	[`consul:1.6.4`](#consul164)
-	[`consul:1.7`](#consul17)
-	[`consul:1.7.3`](#consul173)
-	[`consul:latest`](#consullatest)

## `consul:0.9`

```console
$ docker pull consul@sha256:4ba0f59fc1a0392539e09cb134e2f3b5b6421267007a94854578f2f54e82e0ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:0.9` - linux; amd64

```console
$ docker pull consul@sha256:8646d74af3c4a94a09608d965032033daacebdb9cf6529cfa7f45a08358e62b5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14590256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c3bce3597816e2bfbafaae32957f94339689f34e4430c03eb88c846e94a5fb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 14:18:50 GMT
ENV CONSUL_VERSION=0.9.4
# Fri, 24 Apr 2020 14:18:50 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 14:18:51 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 14:18:54 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 14:18:55 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 14:18:55 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:18:56 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 14:18:56 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 14:18:56 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 14:18:56 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 14:18:56 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:18:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:18:57 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06581be0c8fce2e8ddf90d44df0d6a29224c5dcb31339cda459cc3d486e72b8d`  
		Last Modified: Fri, 24 Apr 2020 14:20:38 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb66ec35f9121e7677d30c091b420ce435d6d47837ee6fbd48b3376c2f317e7`  
		Last Modified: Fri, 24 Apr 2020 14:20:40 GMT  
		Size: 11.8 MB (11813614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a956dd1b0309547d7610dce14fdb95fd4de87b0242ec02249cfef2d431eadd87`  
		Last Modified: Fri, 24 Apr 2020 14:20:38 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2230a0a0602959bfc3437fae33d21276f3def02064f6cefa173f0eb70627b2d3`  
		Last Modified: Fri, 24 Apr 2020 14:20:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49daf8d8264a33688bcddfd7e282d3547ae32d45f9c0a178fb90cd338f856c65`  
		Last Modified: Fri, 24 Apr 2020 14:20:37 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:0.9` - linux; arm variant v6

```console
$ docker pull consul@sha256:7567e9daf88ce6f5c3ff06710d7eb7f9956f4acf0613e2b7579ce5ab92c34eb8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13744277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef19efb76fc0cd13439abe95f8ff14ec99374f710debeaf34e6ac84358d8fadf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Apr 2020 16:58:10 GMT
ENV CONSUL_VERSION=0.9.4
# Thu, 23 Apr 2020 16:58:10 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Apr 2020 16:58:13 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Apr 2020 16:58:19 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Apr 2020 16:58:21 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Apr 2020 16:58:23 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 16:58:24 GMT
VOLUME [/consul/data]
# Thu, 23 Apr 2020 16:58:25 GMT
EXPOSE 8300
# Thu, 23 Apr 2020 16:58:25 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Apr 2020 16:58:26 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Apr 2020 16:58:27 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Apr 2020 16:58:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:58:29 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76cd6ccb5c863262652eb924f8fad144167bc57c0d809638215e0b7ee9fbf24b`  
		Last Modified: Thu, 23 Apr 2020 17:01:16 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e33b1c033f4186a0a18e46808783676a25e443b2ef4db7613505f75e3adb683`  
		Last Modified: Thu, 23 Apr 2020 17:01:19 GMT  
		Size: 11.2 MB (11192262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce2b4a49fbd7a45b7e64b1dc4909e585d0c5ac77bdeb3332b39e3c3538c94bf`  
		Last Modified: Thu, 23 Apr 2020 17:01:16 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92133243f7d8f6ea4f2cc13d1ee9ffcc95daa49bc59fbe68f5015626a5bf0f2`  
		Last Modified: Thu, 23 Apr 2020 17:01:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfe004a5f39aafa0e044b0d38c6724bf0731fdc42d563c3736a01a9541aef70`  
		Last Modified: Thu, 23 Apr 2020 17:01:16 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:0.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:a13440b554925a3090e892c40c4ed986eb1a7b9201eb113f900f17500c73a102
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13789975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:404ce34999a8bdf815a860ef188139d3001304a59af383b79b2ebf4bfad05138`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 09:26:18 GMT
ENV CONSUL_VERSION=0.9.4
# Fri, 24 Apr 2020 09:26:19 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 09:26:21 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 09:26:26 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 09:26:29 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 09:26:31 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 09:26:31 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 09:26:32 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 09:26:33 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 09:26:33 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 09:26:34 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 09:26:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:26:36 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab2f6f245af6ab59413e66a0ae48f525b19912c88fc037fcf2899f42124ed3d`  
		Last Modified: Fri, 24 Apr 2020 09:29:28 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5adb5a8a825ef20b3e29483d4fad5a95a00501d854bbb2059963aab85e01671f`  
		Last Modified: Fri, 24 Apr 2020 09:29:32 GMT  
		Size: 11.1 MB (11092221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb37657561d45f54c0ce34d30d42e501b2a929e6a8aa53891e63908d0daef81`  
		Last Modified: Fri, 24 Apr 2020 09:29:28 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b007c82679f40e214770fdc37821e9cc357a85a1062dd6a0ec8b71b0bd85db`  
		Last Modified: Fri, 24 Apr 2020 09:29:28 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e94889428efe34880702e5d10742fce75f5776a0357d8c94af06b1243b61a3b`  
		Last Modified: Fri, 24 Apr 2020 09:29:28 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:0.9` - linux; 386

```console
$ docker pull consul@sha256:31ea1133901a3a61a3c218f49014fac7707d16a3db9728ccc6c905366ecf2726
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.3 MB (14265875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:585de4ef211624baf2105478bcb70e75a11b0e6afb07bcbd420d456db3abbc6e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 04:32:14 GMT
ENV CONSUL_VERSION=0.9.4
# Fri, 24 Apr 2020 04:32:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 04:32:15 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 04:32:19 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 04:32:19 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 04:32:20 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 04:32:21 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 04:32:21 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 04:32:21 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 04:32:21 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 04:32:21 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 04:32:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:32:22 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3dde02e4ce4dd058fad4111743215f058954357fc76e8e20fb918adc771dfe3`  
		Last Modified: Fri, 24 Apr 2020 04:34:04 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c1e7e0fb63189ec6bfbb90501d4f96dc49953831824701ae5a10ca0491f5cd`  
		Last Modified: Fri, 24 Apr 2020 04:34:07 GMT  
		Size: 11.5 MB (11492906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b85c312c486461e74b80e7b051099d2df0cd64a79c2696da5a1d88e89819cdf`  
		Last Modified: Fri, 24 Apr 2020 04:34:04 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b13c19a5bad8979d00839c34c4d237be507d819433fdb4e4269ff08a37fd95e9`  
		Last Modified: Fri, 24 Apr 2020 04:34:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94136c6ef89b0afa76471ccebd405716f5ddbb1e77c70fd2565218903d226c28`  
		Last Modified: Fri, 24 Apr 2020 04:34:04 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:0.9.4`

```console
$ docker pull consul@sha256:4ba0f59fc1a0392539e09cb134e2f3b5b6421267007a94854578f2f54e82e0ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:0.9.4` - linux; amd64

```console
$ docker pull consul@sha256:8646d74af3c4a94a09608d965032033daacebdb9cf6529cfa7f45a08358e62b5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14590256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c3bce3597816e2bfbafaae32957f94339689f34e4430c03eb88c846e94a5fb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 14:18:50 GMT
ENV CONSUL_VERSION=0.9.4
# Fri, 24 Apr 2020 14:18:50 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 14:18:51 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 14:18:54 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 14:18:55 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 14:18:55 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:18:56 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 14:18:56 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 14:18:56 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 14:18:56 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 14:18:56 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:18:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:18:57 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06581be0c8fce2e8ddf90d44df0d6a29224c5dcb31339cda459cc3d486e72b8d`  
		Last Modified: Fri, 24 Apr 2020 14:20:38 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb66ec35f9121e7677d30c091b420ce435d6d47837ee6fbd48b3376c2f317e7`  
		Last Modified: Fri, 24 Apr 2020 14:20:40 GMT  
		Size: 11.8 MB (11813614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a956dd1b0309547d7610dce14fdb95fd4de87b0242ec02249cfef2d431eadd87`  
		Last Modified: Fri, 24 Apr 2020 14:20:38 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2230a0a0602959bfc3437fae33d21276f3def02064f6cefa173f0eb70627b2d3`  
		Last Modified: Fri, 24 Apr 2020 14:20:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49daf8d8264a33688bcddfd7e282d3547ae32d45f9c0a178fb90cd338f856c65`  
		Last Modified: Fri, 24 Apr 2020 14:20:37 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:0.9.4` - linux; arm variant v6

```console
$ docker pull consul@sha256:7567e9daf88ce6f5c3ff06710d7eb7f9956f4acf0613e2b7579ce5ab92c34eb8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13744277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef19efb76fc0cd13439abe95f8ff14ec99374f710debeaf34e6ac84358d8fadf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Apr 2020 16:58:10 GMT
ENV CONSUL_VERSION=0.9.4
# Thu, 23 Apr 2020 16:58:10 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Apr 2020 16:58:13 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Apr 2020 16:58:19 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Apr 2020 16:58:21 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Apr 2020 16:58:23 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 16:58:24 GMT
VOLUME [/consul/data]
# Thu, 23 Apr 2020 16:58:25 GMT
EXPOSE 8300
# Thu, 23 Apr 2020 16:58:25 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Apr 2020 16:58:26 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Apr 2020 16:58:27 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Apr 2020 16:58:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:58:29 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76cd6ccb5c863262652eb924f8fad144167bc57c0d809638215e0b7ee9fbf24b`  
		Last Modified: Thu, 23 Apr 2020 17:01:16 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e33b1c033f4186a0a18e46808783676a25e443b2ef4db7613505f75e3adb683`  
		Last Modified: Thu, 23 Apr 2020 17:01:19 GMT  
		Size: 11.2 MB (11192262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce2b4a49fbd7a45b7e64b1dc4909e585d0c5ac77bdeb3332b39e3c3538c94bf`  
		Last Modified: Thu, 23 Apr 2020 17:01:16 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92133243f7d8f6ea4f2cc13d1ee9ffcc95daa49bc59fbe68f5015626a5bf0f2`  
		Last Modified: Thu, 23 Apr 2020 17:01:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfe004a5f39aafa0e044b0d38c6724bf0731fdc42d563c3736a01a9541aef70`  
		Last Modified: Thu, 23 Apr 2020 17:01:16 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:0.9.4` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:a13440b554925a3090e892c40c4ed986eb1a7b9201eb113f900f17500c73a102
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13789975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:404ce34999a8bdf815a860ef188139d3001304a59af383b79b2ebf4bfad05138`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 09:26:18 GMT
ENV CONSUL_VERSION=0.9.4
# Fri, 24 Apr 2020 09:26:19 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 09:26:21 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 09:26:26 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 09:26:29 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 09:26:31 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 09:26:31 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 09:26:32 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 09:26:33 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 09:26:33 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 09:26:34 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 09:26:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:26:36 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab2f6f245af6ab59413e66a0ae48f525b19912c88fc037fcf2899f42124ed3d`  
		Last Modified: Fri, 24 Apr 2020 09:29:28 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5adb5a8a825ef20b3e29483d4fad5a95a00501d854bbb2059963aab85e01671f`  
		Last Modified: Fri, 24 Apr 2020 09:29:32 GMT  
		Size: 11.1 MB (11092221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb37657561d45f54c0ce34d30d42e501b2a929e6a8aa53891e63908d0daef81`  
		Last Modified: Fri, 24 Apr 2020 09:29:28 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b007c82679f40e214770fdc37821e9cc357a85a1062dd6a0ec8b71b0bd85db`  
		Last Modified: Fri, 24 Apr 2020 09:29:28 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e94889428efe34880702e5d10742fce75f5776a0357d8c94af06b1243b61a3b`  
		Last Modified: Fri, 24 Apr 2020 09:29:28 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:0.9.4` - linux; 386

```console
$ docker pull consul@sha256:31ea1133901a3a61a3c218f49014fac7707d16a3db9728ccc6c905366ecf2726
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.3 MB (14265875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:585de4ef211624baf2105478bcb70e75a11b0e6afb07bcbd420d456db3abbc6e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 04:32:14 GMT
ENV CONSUL_VERSION=0.9.4
# Fri, 24 Apr 2020 04:32:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 04:32:15 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 04:32:19 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 04:32:19 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 04:32:20 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 04:32:21 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 04:32:21 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 04:32:21 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 04:32:21 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 04:32:21 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 04:32:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:32:22 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3dde02e4ce4dd058fad4111743215f058954357fc76e8e20fb918adc771dfe3`  
		Last Modified: Fri, 24 Apr 2020 04:34:04 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c1e7e0fb63189ec6bfbb90501d4f96dc49953831824701ae5a10ca0491f5cd`  
		Last Modified: Fri, 24 Apr 2020 04:34:07 GMT  
		Size: 11.5 MB (11492906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b85c312c486461e74b80e7b051099d2df0cd64a79c2696da5a1d88e89819cdf`  
		Last Modified: Fri, 24 Apr 2020 04:34:04 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b13c19a5bad8979d00839c34c4d237be507d819433fdb4e4269ff08a37fd95e9`  
		Last Modified: Fri, 24 Apr 2020 04:34:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94136c6ef89b0afa76471ccebd405716f5ddbb1e77c70fd2565218903d226c28`  
		Last Modified: Fri, 24 Apr 2020 04:34:04 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.0`

```console
$ docker pull consul@sha256:87bef0dd0b4334a560bfab978d92e3b36c2124703a5ddb44cd5917b2ba4c7f96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.0` - linux; amd64

```console
$ docker pull consul@sha256:23fefc444298d71ad2000f224f851ce7677a147fcf9a51505972341bb98af828
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16604256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d8161cc967510f94c8138272ae1f8fd941ca7e64c2d05c42718a108a78dd210`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 14:18:39 GMT
ENV CONSUL_VERSION=1.0.8
# Fri, 24 Apr 2020 14:18:39 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 14:18:40 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 14:18:43 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 14:18:44 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 14:18:45 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:18:45 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 14:18:45 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 14:18:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 14:18:45 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 14:18:45 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:18:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:18:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a175f9e722e4499bcd8d1f24912559efa6ac03dc87b03ac0e6ec47a6044a4e12`  
		Last Modified: Fri, 24 Apr 2020 14:20:30 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9a43f101c642d6477bb6335402beb30a881e9948a751d917c836e752a36efd`  
		Last Modified: Fri, 24 Apr 2020 14:20:33 GMT  
		Size: 13.8 MB (13827612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7197b0ced71da3016ff111b9e656f2ef08fe3c3eaf49e52c18c808d4067bad35`  
		Last Modified: Fri, 24 Apr 2020 14:20:30 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712469348d05219c9dcd60b60a509dcf8e78d135d8db6ea1092218437509b073`  
		Last Modified: Fri, 24 Apr 2020 14:20:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d67797597fb41f37713cf82e5fd545d0c4be3be5420ceaec1c3aa8ae3850ae`  
		Last Modified: Fri, 24 Apr 2020 14:20:30 GMT  
		Size: 1.7 KB (1681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.0` - linux; arm variant v6

```console
$ docker pull consul@sha256:8ed068a4e959077cf3763ea930cafdfa67faad921b172d853c503548fa23b09f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15927267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4a8ea9bd4bd84c23339c822cc1d664f27f2fb430d174cd40a15ddd102098268`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Apr 2020 16:57:39 GMT
ENV CONSUL_VERSION=1.0.8
# Thu, 23 Apr 2020 16:57:40 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Apr 2020 16:57:42 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Apr 2020 16:57:49 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Apr 2020 16:57:55 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Apr 2020 16:57:58 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 16:57:58 GMT
VOLUME [/consul/data]
# Thu, 23 Apr 2020 16:57:59 GMT
EXPOSE 8300
# Thu, 23 Apr 2020 16:58:00 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Apr 2020 16:58:01 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Apr 2020 16:58:02 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Apr 2020 16:58:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:58:03 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7f1ec021b4538db3c83f84b62bb94da1519016e0073c4f5148322e57043678`  
		Last Modified: Thu, 23 Apr 2020 17:01:02 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1d832c9019f7acf2ca2a1b554704ed90a4fd3815998118c9ab8f2d5700daa0`  
		Last Modified: Thu, 23 Apr 2020 17:01:07 GMT  
		Size: 13.4 MB (13375251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1973747b0151219f88c7cab68412c0aaa44445791287c96a838bc3d0cca8018e`  
		Last Modified: Thu, 23 Apr 2020 17:01:01 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50cb5fffaf1ddd735c3e52e4ca181126c92329f3d43ef2cb6b38869f87e661a`  
		Last Modified: Thu, 23 Apr 2020 17:01:02 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f475845735cc1de22cdcb0faeadf59b78ecbb89fe44f32adcc5986d73eaae827`  
		Last Modified: Thu, 23 Apr 2020 17:01:02 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.0` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:285cfcf7d8317709e6dc46de81977598df3095ecd6c5c2795842e41c1330f074
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15938163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f12784b06afc03511df3e731d0e01184c2b05ecedce581c3e27cef1c8cee149`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 09:25:51 GMT
ENV CONSUL_VERSION=1.0.8
# Fri, 24 Apr 2020 09:25:52 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 09:25:54 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 09:25:59 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 09:26:03 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 09:26:05 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 09:26:05 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 09:26:06 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 09:26:07 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 09:26:08 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 09:26:09 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 09:26:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:26:10 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad7d2b93ab1eb5a34e6982495f0a2bb5893db041369278bad9a208f54ffcc37`  
		Last Modified: Fri, 24 Apr 2020 09:29:15 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11fcae0383ed139ed92a0e0f9d04425c9162949246201fccebefcdcbfa33281d`  
		Last Modified: Fri, 24 Apr 2020 09:29:19 GMT  
		Size: 13.2 MB (13240403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9ee512a3a0d4fa56fc8fdf4f14b06d464d936ed52abf0b7f9291e4792116cc`  
		Last Modified: Fri, 24 Apr 2020 09:29:15 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d49e932f1e3560cce2811c1da9fb185aa5148e3993ce5243483dba1ca72111`  
		Last Modified: Fri, 24 Apr 2020 09:29:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8026929bfbb48a0798d5571ea44263c5fc1203f9ee229d0f83a05c384c90a7ad`  
		Last Modified: Fri, 24 Apr 2020 09:29:15 GMT  
		Size: 1.7 KB (1680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.0` - linux; 386

```console
$ docker pull consul@sha256:1d77c81c3039fad28156b6e55137082061933af879bac32bdf2793ea8fad9f8a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16488482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0d131c2161d7707dc210fe3845fa107d1bdf531574631e8ae38a417c3b9198`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 04:32:04 GMT
ENV CONSUL_VERSION=1.0.8
# Fri, 24 Apr 2020 04:32:04 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 04:32:05 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 04:32:08 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 04:32:09 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 04:32:10 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 04:32:10 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 04:32:10 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 04:32:10 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 04:32:10 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 04:32:11 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 04:32:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:32:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850240b833ceb1a2c21f19767158367cc05e0dfce3b9ab8400783540669769d3`  
		Last Modified: Fri, 24 Apr 2020 04:33:55 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c56ab7d56e42aabf7140922618da2a3da26d2ca704983eeafa728c0c1e91c1`  
		Last Modified: Fri, 24 Apr 2020 04:33:59 GMT  
		Size: 13.7 MB (13715515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16846dd8889e312196cb104f75ff12d5ebfebc6e9e0e4d6009ba0f3e8f1c464`  
		Last Modified: Fri, 24 Apr 2020 04:33:55 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b35ea71b0133f4d25007c58be12051c0cfd1ecc56c0319920da065e220f7ed6`  
		Last Modified: Fri, 24 Apr 2020 04:33:55 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a089445a55f289bec444acc9e912f021d47dcd4e8c6c3a9c7d05bdf6d4fb03`  
		Last Modified: Fri, 24 Apr 2020 04:33:55 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.0.8`

```console
$ docker pull consul@sha256:87bef0dd0b4334a560bfab978d92e3b36c2124703a5ddb44cd5917b2ba4c7f96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.0.8` - linux; amd64

```console
$ docker pull consul@sha256:23fefc444298d71ad2000f224f851ce7677a147fcf9a51505972341bb98af828
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16604256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d8161cc967510f94c8138272ae1f8fd941ca7e64c2d05c42718a108a78dd210`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 14:18:39 GMT
ENV CONSUL_VERSION=1.0.8
# Fri, 24 Apr 2020 14:18:39 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 14:18:40 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 14:18:43 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 14:18:44 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 14:18:45 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:18:45 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 14:18:45 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 14:18:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 14:18:45 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 14:18:45 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:18:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:18:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a175f9e722e4499bcd8d1f24912559efa6ac03dc87b03ac0e6ec47a6044a4e12`  
		Last Modified: Fri, 24 Apr 2020 14:20:30 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9a43f101c642d6477bb6335402beb30a881e9948a751d917c836e752a36efd`  
		Last Modified: Fri, 24 Apr 2020 14:20:33 GMT  
		Size: 13.8 MB (13827612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7197b0ced71da3016ff111b9e656f2ef08fe3c3eaf49e52c18c808d4067bad35`  
		Last Modified: Fri, 24 Apr 2020 14:20:30 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712469348d05219c9dcd60b60a509dcf8e78d135d8db6ea1092218437509b073`  
		Last Modified: Fri, 24 Apr 2020 14:20:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d67797597fb41f37713cf82e5fd545d0c4be3be5420ceaec1c3aa8ae3850ae`  
		Last Modified: Fri, 24 Apr 2020 14:20:30 GMT  
		Size: 1.7 KB (1681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.0.8` - linux; arm variant v6

```console
$ docker pull consul@sha256:8ed068a4e959077cf3763ea930cafdfa67faad921b172d853c503548fa23b09f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15927267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4a8ea9bd4bd84c23339c822cc1d664f27f2fb430d174cd40a15ddd102098268`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Apr 2020 16:57:39 GMT
ENV CONSUL_VERSION=1.0.8
# Thu, 23 Apr 2020 16:57:40 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Apr 2020 16:57:42 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Apr 2020 16:57:49 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Apr 2020 16:57:55 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Apr 2020 16:57:58 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 16:57:58 GMT
VOLUME [/consul/data]
# Thu, 23 Apr 2020 16:57:59 GMT
EXPOSE 8300
# Thu, 23 Apr 2020 16:58:00 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Apr 2020 16:58:01 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Apr 2020 16:58:02 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Apr 2020 16:58:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:58:03 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7f1ec021b4538db3c83f84b62bb94da1519016e0073c4f5148322e57043678`  
		Last Modified: Thu, 23 Apr 2020 17:01:02 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1d832c9019f7acf2ca2a1b554704ed90a4fd3815998118c9ab8f2d5700daa0`  
		Last Modified: Thu, 23 Apr 2020 17:01:07 GMT  
		Size: 13.4 MB (13375251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1973747b0151219f88c7cab68412c0aaa44445791287c96a838bc3d0cca8018e`  
		Last Modified: Thu, 23 Apr 2020 17:01:01 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50cb5fffaf1ddd735c3e52e4ca181126c92329f3d43ef2cb6b38869f87e661a`  
		Last Modified: Thu, 23 Apr 2020 17:01:02 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f475845735cc1de22cdcb0faeadf59b78ecbb89fe44f32adcc5986d73eaae827`  
		Last Modified: Thu, 23 Apr 2020 17:01:02 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.0.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:285cfcf7d8317709e6dc46de81977598df3095ecd6c5c2795842e41c1330f074
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15938163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f12784b06afc03511df3e731d0e01184c2b05ecedce581c3e27cef1c8cee149`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 09:25:51 GMT
ENV CONSUL_VERSION=1.0.8
# Fri, 24 Apr 2020 09:25:52 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 09:25:54 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 09:25:59 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 09:26:03 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 09:26:05 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 09:26:05 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 09:26:06 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 09:26:07 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 09:26:08 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 09:26:09 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 09:26:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:26:10 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad7d2b93ab1eb5a34e6982495f0a2bb5893db041369278bad9a208f54ffcc37`  
		Last Modified: Fri, 24 Apr 2020 09:29:15 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11fcae0383ed139ed92a0e0f9d04425c9162949246201fccebefcdcbfa33281d`  
		Last Modified: Fri, 24 Apr 2020 09:29:19 GMT  
		Size: 13.2 MB (13240403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9ee512a3a0d4fa56fc8fdf4f14b06d464d936ed52abf0b7f9291e4792116cc`  
		Last Modified: Fri, 24 Apr 2020 09:29:15 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d49e932f1e3560cce2811c1da9fb185aa5148e3993ce5243483dba1ca72111`  
		Last Modified: Fri, 24 Apr 2020 09:29:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8026929bfbb48a0798d5571ea44263c5fc1203f9ee229d0f83a05c384c90a7ad`  
		Last Modified: Fri, 24 Apr 2020 09:29:15 GMT  
		Size: 1.7 KB (1680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.0.8` - linux; 386

```console
$ docker pull consul@sha256:1d77c81c3039fad28156b6e55137082061933af879bac32bdf2793ea8fad9f8a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16488482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0d131c2161d7707dc210fe3845fa107d1bdf531574631e8ae38a417c3b9198`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 04:32:04 GMT
ENV CONSUL_VERSION=1.0.8
# Fri, 24 Apr 2020 04:32:04 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 04:32:05 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 04:32:08 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 04:32:09 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 04:32:10 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 04:32:10 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 04:32:10 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 04:32:10 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 04:32:10 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 04:32:11 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 04:32:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:32:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850240b833ceb1a2c21f19767158367cc05e0dfce3b9ab8400783540669769d3`  
		Last Modified: Fri, 24 Apr 2020 04:33:55 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c56ab7d56e42aabf7140922618da2a3da26d2ca704983eeafa728c0c1e91c1`  
		Last Modified: Fri, 24 Apr 2020 04:33:59 GMT  
		Size: 13.7 MB (13715515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16846dd8889e312196cb104f75ff12d5ebfebc6e9e0e4d6009ba0f3e8f1c464`  
		Last Modified: Fri, 24 Apr 2020 04:33:55 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b35ea71b0133f4d25007c58be12051c0cfd1ecc56c0319920da065e220f7ed6`  
		Last Modified: Fri, 24 Apr 2020 04:33:55 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a089445a55f289bec444acc9e912f021d47dcd4e8c6c3a9c7d05bdf6d4fb03`  
		Last Modified: Fri, 24 Apr 2020 04:33:55 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.1`

```console
$ docker pull consul@sha256:634109ced53da72535e4dae663d17bb7207169974c8114e468fc9b7a4b06c0a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.1` - linux; amd64

```console
$ docker pull consul@sha256:c02228a7ffa3c276eb7ede6d460b518bbf4580c65ecf86bae4da3ea69d4b4808
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.1 MB (18069429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d01fdc265b5eba39e8c07cbf4939f15960e993cba7db2a5419a439d1aad33c6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 14:18:28 GMT
ENV CONSUL_VERSION=1.1.1
# Fri, 24 Apr 2020 14:18:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 14:18:29 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 14:18:32 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 14:18:33 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 14:18:34 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:18:34 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 14:18:34 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 14:18:34 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 14:18:35 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 14:18:35 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:18:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:18:35 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff03907c9c3cab2dc21ca0fae08afebbcf0ef856d3815f113cc31cedec93eb1`  
		Last Modified: Fri, 24 Apr 2020 14:20:23 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1cec3bc85977b40076523141a913f9b0ce2d784081402600db86e350c3c1c64`  
		Last Modified: Fri, 24 Apr 2020 14:20:26 GMT  
		Size: 15.3 MB (15292791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e70648ae8f73312eb482f0b1be734dad75dc265f6f9f34a6f0021298e8a0df`  
		Last Modified: Fri, 24 Apr 2020 14:20:24 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4457d93ceac0f759d4ffde34ed340d9bd0e7377953391382191d36866e59209`  
		Last Modified: Fri, 24 Apr 2020 14:20:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662bf62f8bc1b12f571f856e2a81bfd75bac3781206f312f2dcb5f63a984ade0`  
		Last Modified: Fri, 24 Apr 2020 14:20:24 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.1` - linux; arm variant v6

```console
$ docker pull consul@sha256:a0fa5de1a39eed6614e477f3e3319c99495493dd5d5c1e8b74bbc94e0db62bdb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17390617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d02828dfd615d155ebe7e24a956db44dba5c23d3b32d55bd6e4f0a3957602eee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Apr 2020 16:57:03 GMT
ENV CONSUL_VERSION=1.1.1
# Thu, 23 Apr 2020 16:57:04 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Apr 2020 16:57:05 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Apr 2020 16:57:12 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Apr 2020 16:57:21 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Apr 2020 16:57:25 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 16:57:26 GMT
VOLUME [/consul/data]
# Thu, 23 Apr 2020 16:57:26 GMT
EXPOSE 8300
# Thu, 23 Apr 2020 16:57:27 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Apr 2020 16:57:28 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Apr 2020 16:57:28 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Apr 2020 16:57:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:57:29 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1a16aa19bbf6b544dc6929c42ee2bdd9f4e744998365e9c33316b04c835ada`  
		Last Modified: Thu, 23 Apr 2020 17:00:50 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f49072c61926a893f1cab6572bcafbc9879a83b81b4cc9f7ce195723a64ac2`  
		Last Modified: Thu, 23 Apr 2020 17:00:55 GMT  
		Size: 14.8 MB (14838606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb7df641eaf55de68bf5895395ab1b3226e4f5b0b0a529021349bfb8099e36e`  
		Last Modified: Thu, 23 Apr 2020 17:00:50 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b10f5e9dee1a269b0d214de927b08485c0139d30e80396f9b061d589aee59e`  
		Last Modified: Thu, 23 Apr 2020 17:00:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7c40f6de602110916c804223738d168850c5db10e634ef04a8a4e8f7e71350`  
		Last Modified: Thu, 23 Apr 2020 17:00:50 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.1` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:44f289ef036424b2d8ce04ac39ded7c414757febc3d6cc53b998dbdf8d21cd22
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17374389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:208aa3e3b738f250c890c324a9a4fd960cc9cec7f30c7f7d58e63fb208ee4242`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 09:25:15 GMT
ENV CONSUL_VERSION=1.1.1
# Fri, 24 Apr 2020 09:25:16 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 09:25:18 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 09:25:23 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 09:25:26 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 09:25:30 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 09:25:35 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 09:25:36 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 09:25:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 09:25:39 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 09:25:41 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 09:25:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:25:43 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5201feb5d74971db84455fc28f544bed1b0197f70865c92b40ca28a546d368a`  
		Last Modified: Fri, 24 Apr 2020 09:29:01 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b76ccf1fa98d761f9331c88497071b058441aab88293490be7c779c22ec5c54`  
		Last Modified: Fri, 24 Apr 2020 09:29:06 GMT  
		Size: 14.7 MB (14676628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df09f2f2998409912f9ba46762c820be324a6f2080501f487ecfbcf25f564d78`  
		Last Modified: Fri, 24 Apr 2020 09:29:01 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1402e1ea3eceb233f63773e4f8b629c924bd17a98233ed05c6b7f6b2ef1afa`  
		Last Modified: Fri, 24 Apr 2020 09:29:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684a1f16ecc1f40594ba9be38075648723f1c36583dd74a412d5721d2458812d`  
		Last Modified: Fri, 24 Apr 2020 09:29:01 GMT  
		Size: 1.7 KB (1681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.1` - linux; 386

```console
$ docker pull consul@sha256:e1a43e2d64d69c8d3653ee646430183e08556e6feac71e79beb0015c7eafd8e4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.0 MB (17960253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd7b4ecea4861c81a2ed5fd1ec5222d0802c39a3c66efc6e147dcd6b056cd931`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 04:31:53 GMT
ENV CONSUL_VERSION=1.1.1
# Fri, 24 Apr 2020 04:31:53 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 04:31:54 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 04:31:57 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 04:31:58 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 04:31:59 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 04:31:59 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 04:31:59 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 04:31:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 04:31:59 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 04:32:00 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 04:32:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:32:00 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29818b9044046d6411c4fc801bc923c8c1b927e298e7ab2dc918a838551d939`  
		Last Modified: Fri, 24 Apr 2020 04:33:41 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82024872e9d3c48b8ecf7cee0fa0cb357e20c4a5d47aae161597e702689529f1`  
		Last Modified: Fri, 24 Apr 2020 04:33:44 GMT  
		Size: 15.2 MB (15187288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9848c4a2e774d7260fd7abd8bf55c21b93d4739a5d97d669f3a4415854e1f65a`  
		Last Modified: Fri, 24 Apr 2020 04:33:40 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fccc47ff63aef6639dcec62889f890b94c256ee6ced64bd35573e0081810c0e6`  
		Last Modified: Fri, 24 Apr 2020 04:33:41 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce866c09d565e3efb843bc7c65209d46b5acc12a8a922c95b12f72a13ac1de67`  
		Last Modified: Fri, 24 Apr 2020 04:33:40 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.1.1`

```console
$ docker pull consul@sha256:634109ced53da72535e4dae663d17bb7207169974c8114e468fc9b7a4b06c0a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.1.1` - linux; amd64

```console
$ docker pull consul@sha256:c02228a7ffa3c276eb7ede6d460b518bbf4580c65ecf86bae4da3ea69d4b4808
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.1 MB (18069429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d01fdc265b5eba39e8c07cbf4939f15960e993cba7db2a5419a439d1aad33c6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 14:18:28 GMT
ENV CONSUL_VERSION=1.1.1
# Fri, 24 Apr 2020 14:18:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 14:18:29 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 14:18:32 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 14:18:33 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 14:18:34 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:18:34 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 14:18:34 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 14:18:34 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 14:18:35 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 14:18:35 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:18:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:18:35 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff03907c9c3cab2dc21ca0fae08afebbcf0ef856d3815f113cc31cedec93eb1`  
		Last Modified: Fri, 24 Apr 2020 14:20:23 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1cec3bc85977b40076523141a913f9b0ce2d784081402600db86e350c3c1c64`  
		Last Modified: Fri, 24 Apr 2020 14:20:26 GMT  
		Size: 15.3 MB (15292791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e70648ae8f73312eb482f0b1be734dad75dc265f6f9f34a6f0021298e8a0df`  
		Last Modified: Fri, 24 Apr 2020 14:20:24 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4457d93ceac0f759d4ffde34ed340d9bd0e7377953391382191d36866e59209`  
		Last Modified: Fri, 24 Apr 2020 14:20:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662bf62f8bc1b12f571f856e2a81bfd75bac3781206f312f2dcb5f63a984ade0`  
		Last Modified: Fri, 24 Apr 2020 14:20:24 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.1.1` - linux; arm variant v6

```console
$ docker pull consul@sha256:a0fa5de1a39eed6614e477f3e3319c99495493dd5d5c1e8b74bbc94e0db62bdb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17390617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d02828dfd615d155ebe7e24a956db44dba5c23d3b32d55bd6e4f0a3957602eee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Apr 2020 16:57:03 GMT
ENV CONSUL_VERSION=1.1.1
# Thu, 23 Apr 2020 16:57:04 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Apr 2020 16:57:05 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Apr 2020 16:57:12 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Apr 2020 16:57:21 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Apr 2020 16:57:25 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 16:57:26 GMT
VOLUME [/consul/data]
# Thu, 23 Apr 2020 16:57:26 GMT
EXPOSE 8300
# Thu, 23 Apr 2020 16:57:27 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Apr 2020 16:57:28 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Apr 2020 16:57:28 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Apr 2020 16:57:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:57:29 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1a16aa19bbf6b544dc6929c42ee2bdd9f4e744998365e9c33316b04c835ada`  
		Last Modified: Thu, 23 Apr 2020 17:00:50 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f49072c61926a893f1cab6572bcafbc9879a83b81b4cc9f7ce195723a64ac2`  
		Last Modified: Thu, 23 Apr 2020 17:00:55 GMT  
		Size: 14.8 MB (14838606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb7df641eaf55de68bf5895395ab1b3226e4f5b0b0a529021349bfb8099e36e`  
		Last Modified: Thu, 23 Apr 2020 17:00:50 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b10f5e9dee1a269b0d214de927b08485c0139d30e80396f9b061d589aee59e`  
		Last Modified: Thu, 23 Apr 2020 17:00:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7c40f6de602110916c804223738d168850c5db10e634ef04a8a4e8f7e71350`  
		Last Modified: Thu, 23 Apr 2020 17:00:50 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.1.1` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:44f289ef036424b2d8ce04ac39ded7c414757febc3d6cc53b998dbdf8d21cd22
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17374389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:208aa3e3b738f250c890c324a9a4fd960cc9cec7f30c7f7d58e63fb208ee4242`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 09:25:15 GMT
ENV CONSUL_VERSION=1.1.1
# Fri, 24 Apr 2020 09:25:16 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 09:25:18 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 09:25:23 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 09:25:26 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 09:25:30 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 09:25:35 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 09:25:36 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 09:25:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 09:25:39 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 09:25:41 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 09:25:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:25:43 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5201feb5d74971db84455fc28f544bed1b0197f70865c92b40ca28a546d368a`  
		Last Modified: Fri, 24 Apr 2020 09:29:01 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b76ccf1fa98d761f9331c88497071b058441aab88293490be7c779c22ec5c54`  
		Last Modified: Fri, 24 Apr 2020 09:29:06 GMT  
		Size: 14.7 MB (14676628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df09f2f2998409912f9ba46762c820be324a6f2080501f487ecfbcf25f564d78`  
		Last Modified: Fri, 24 Apr 2020 09:29:01 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1402e1ea3eceb233f63773e4f8b629c924bd17a98233ed05c6b7f6b2ef1afa`  
		Last Modified: Fri, 24 Apr 2020 09:29:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684a1f16ecc1f40594ba9be38075648723f1c36583dd74a412d5721d2458812d`  
		Last Modified: Fri, 24 Apr 2020 09:29:01 GMT  
		Size: 1.7 KB (1681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.1.1` - linux; 386

```console
$ docker pull consul@sha256:e1a43e2d64d69c8d3653ee646430183e08556e6feac71e79beb0015c7eafd8e4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.0 MB (17960253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd7b4ecea4861c81a2ed5fd1ec5222d0802c39a3c66efc6e147dcd6b056cd931`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 04:31:53 GMT
ENV CONSUL_VERSION=1.1.1
# Fri, 24 Apr 2020 04:31:53 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 04:31:54 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 04:31:57 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 04:31:58 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 04:31:59 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 04:31:59 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 04:31:59 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 04:31:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 04:31:59 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 04:32:00 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 04:32:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:32:00 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29818b9044046d6411c4fc801bc923c8c1b927e298e7ab2dc918a838551d939`  
		Last Modified: Fri, 24 Apr 2020 04:33:41 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82024872e9d3c48b8ecf7cee0fa0cb357e20c4a5d47aae161597e702689529f1`  
		Last Modified: Fri, 24 Apr 2020 04:33:44 GMT  
		Size: 15.2 MB (15187288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9848c4a2e774d7260fd7abd8bf55c21b93d4739a5d97d669f3a4415854e1f65a`  
		Last Modified: Fri, 24 Apr 2020 04:33:40 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fccc47ff63aef6639dcec62889f890b94c256ee6ced64bd35573e0081810c0e6`  
		Last Modified: Fri, 24 Apr 2020 04:33:41 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce866c09d565e3efb843bc7c65209d46b5acc12a8a922c95b12f72a13ac1de67`  
		Last Modified: Fri, 24 Apr 2020 04:33:40 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.2`

```console
$ docker pull consul@sha256:8b8d6c80125e7ad97c3eddbf0f0f492b902f16a5ff86ba575cfe4cb873d79df9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.2` - linux; amd64

```console
$ docker pull consul@sha256:c3b794a30301b4252c8e6582f35864e0440d735799aedb6be1f23ce60b77a8a3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28368501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bce376ead4a9c33c6ee6d84252423f5febbbf7c8b056b5ec0101e7b8dbaada5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 14:18:16 GMT
ENV CONSUL_VERSION=1.2.4
# Fri, 24 Apr 2020 14:18:16 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 14:18:17 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 14:18:21 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 14:18:22 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 14:18:23 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:18:23 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 14:18:23 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 14:18:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 14:18:23 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 14:18:24 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:18:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:18:24 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52ee602e4e80ce98227a290d7c0a5b07da64441ad13dc83b7811182594b7655`  
		Last Modified: Fri, 24 Apr 2020 14:20:12 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84a965550ebe7941bb69adee5a6da926bc4eb7fc35604d95af61c69183fc8bd`  
		Last Modified: Fri, 24 Apr 2020 14:20:17 GMT  
		Size: 25.6 MB (25591858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0d2c7496f41017fd84f0e7052f733373253f2533a315005e03e7dbb8382d68`  
		Last Modified: Fri, 24 Apr 2020 14:20:12 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9f67d73030ade44c718c6deeee1d7fd73635927194ca8270ab79462c6e2e50`  
		Last Modified: Fri, 24 Apr 2020 14:20:12 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35b21201bcf5fbd634b91c5fa2babe5da90cb4f428a05d9ae6eb22c74534d76`  
		Last Modified: Fri, 24 Apr 2020 14:20:12 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.2` - linux; arm variant v6

```console
$ docker pull consul@sha256:0d6f34d42d8c26690901030ac0382f77be4afaa8ad4706286860e8944088f9fe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27345781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad66141a43a06cc1daa7be94e6c1610972ea616993dc0ef2e59cdeb0fdc4b9c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Apr 2020 16:56:21 GMT
ENV CONSUL_VERSION=1.2.4
# Thu, 23 Apr 2020 16:56:23 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Apr 2020 16:56:28 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Apr 2020 16:56:38 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Apr 2020 16:56:41 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Apr 2020 16:56:43 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 16:56:44 GMT
VOLUME [/consul/data]
# Thu, 23 Apr 2020 16:56:45 GMT
EXPOSE 8300
# Thu, 23 Apr 2020 16:56:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Apr 2020 16:56:47 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Apr 2020 16:56:48 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Apr 2020 16:56:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:56:51 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f3902c6755e51bc4deae181fb9e3f445726058a580540b34180b1d901bc6ad`  
		Last Modified: Thu, 23 Apr 2020 17:00:31 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d2907d69059834ae38df9cb5ce5abea2286c44944108ddc8df3b64d2072e3c`  
		Last Modified: Thu, 23 Apr 2020 17:00:42 GMT  
		Size: 24.8 MB (24793766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5639b6974ec6a0586ead06dbf648a68278de4759d13602db9a1829dc2cb25d75`  
		Last Modified: Thu, 23 Apr 2020 17:00:30 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39db0dc08d2fae5a5b6e0fb7f21074ba1438c9b266a6d744c8b6f8822e742bca`  
		Last Modified: Thu, 23 Apr 2020 17:00:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebcc61ca2620bd4f870fb0a74fdb77fcb9537c8db1fd17e40ab67a24ebc32e5`  
		Last Modified: Thu, 23 Apr 2020 17:00:30 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.2` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:d75f7d848405d07dea8af762cf052d029d05fc1ab3bb4d6bd42350b7af3f0808
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27145107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8037eab95b5e362188fb87562d495196b651ea499864f85b0e0945a5e907d26b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 09:24:49 GMT
ENV CONSUL_VERSION=1.2.4
# Fri, 24 Apr 2020 09:24:50 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 09:24:52 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 09:24:58 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 09:25:01 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 09:25:02 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 09:25:03 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 09:25:04 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 09:25:05 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 09:25:05 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 09:25:06 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 09:25:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:25:07 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9135996ebc8c26008490ea9eaeaf2d33a092ddb9b862addf499efb68255318d`  
		Last Modified: Fri, 24 Apr 2020 09:28:44 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d97bb3b4d363ddaf4744bf99247a774be1a9b2e2c23a21d4630d46825b6b4609`  
		Last Modified: Fri, 24 Apr 2020 09:28:52 GMT  
		Size: 24.4 MB (24447349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89eab74816070ac224055298a4354d0203ff72cde9ce635df82723ef700c9d49`  
		Last Modified: Fri, 24 Apr 2020 09:28:44 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301bd6c0ecfe81d7f5d130a8f8bc2214b721497c36fd9750a88ba4d07821c39a`  
		Last Modified: Fri, 24 Apr 2020 09:28:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc19ecd92f930789f56504c740bd2832784e2af968c57c8adcceea3a4478deee`  
		Last Modified: Fri, 24 Apr 2020 09:28:44 GMT  
		Size: 1.7 KB (1679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.2` - linux; 386

```console
$ docker pull consul@sha256:b9a93a22356863237ed47a3692f6e2fc40a5b0fa5e3d8b8c95f76ba507cdc9db
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28101751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e3e502fdb651377d03b343346bda8d434d8718463104359331977ee30ed7bbd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 04:31:40 GMT
ENV CONSUL_VERSION=1.2.4
# Fri, 24 Apr 2020 04:31:41 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 04:31:41 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 04:31:46 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 04:31:47 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 04:31:48 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 04:31:48 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 04:31:48 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 04:31:48 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 04:31:48 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 04:31:49 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 04:31:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:31:49 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cdc7080aa5cc8080f04d30e5771a15fbf5d8d6dd249e30fb0039e632a12c856`  
		Last Modified: Fri, 24 Apr 2020 04:33:30 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee895264375d68e371e42de8cdb7676ede8f2201c9d50f0a794d8cc7065eb56`  
		Last Modified: Fri, 24 Apr 2020 04:33:36 GMT  
		Size: 25.3 MB (25328787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b88d9a79f4beb250b040b661aa73be2a783b1b2c85e25577546c1187245ac3`  
		Last Modified: Fri, 24 Apr 2020 04:33:30 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e95e69b1d54b002d348a2c673da9bcc4688a23a90f0d8d91d8a584cd72bec7`  
		Last Modified: Fri, 24 Apr 2020 04:33:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddd71981e8a6865516e8d14d62639591c70baaee9bb2e595a73b30fca471616`  
		Last Modified: Fri, 24 Apr 2020 04:33:30 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.2.4`

```console
$ docker pull consul@sha256:8b8d6c80125e7ad97c3eddbf0f0f492b902f16a5ff86ba575cfe4cb873d79df9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.2.4` - linux; amd64

```console
$ docker pull consul@sha256:c3b794a30301b4252c8e6582f35864e0440d735799aedb6be1f23ce60b77a8a3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28368501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bce376ead4a9c33c6ee6d84252423f5febbbf7c8b056b5ec0101e7b8dbaada5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 14:18:16 GMT
ENV CONSUL_VERSION=1.2.4
# Fri, 24 Apr 2020 14:18:16 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 14:18:17 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 14:18:21 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 14:18:22 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 14:18:23 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:18:23 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 14:18:23 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 14:18:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 14:18:23 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 14:18:24 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:18:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:18:24 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52ee602e4e80ce98227a290d7c0a5b07da64441ad13dc83b7811182594b7655`  
		Last Modified: Fri, 24 Apr 2020 14:20:12 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84a965550ebe7941bb69adee5a6da926bc4eb7fc35604d95af61c69183fc8bd`  
		Last Modified: Fri, 24 Apr 2020 14:20:17 GMT  
		Size: 25.6 MB (25591858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0d2c7496f41017fd84f0e7052f733373253f2533a315005e03e7dbb8382d68`  
		Last Modified: Fri, 24 Apr 2020 14:20:12 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9f67d73030ade44c718c6deeee1d7fd73635927194ca8270ab79462c6e2e50`  
		Last Modified: Fri, 24 Apr 2020 14:20:12 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35b21201bcf5fbd634b91c5fa2babe5da90cb4f428a05d9ae6eb22c74534d76`  
		Last Modified: Fri, 24 Apr 2020 14:20:12 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.2.4` - linux; arm variant v6

```console
$ docker pull consul@sha256:0d6f34d42d8c26690901030ac0382f77be4afaa8ad4706286860e8944088f9fe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27345781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad66141a43a06cc1daa7be94e6c1610972ea616993dc0ef2e59cdeb0fdc4b9c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Apr 2020 16:56:21 GMT
ENV CONSUL_VERSION=1.2.4
# Thu, 23 Apr 2020 16:56:23 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Apr 2020 16:56:28 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Apr 2020 16:56:38 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Apr 2020 16:56:41 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Apr 2020 16:56:43 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 16:56:44 GMT
VOLUME [/consul/data]
# Thu, 23 Apr 2020 16:56:45 GMT
EXPOSE 8300
# Thu, 23 Apr 2020 16:56:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Apr 2020 16:56:47 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Apr 2020 16:56:48 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Apr 2020 16:56:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:56:51 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f3902c6755e51bc4deae181fb9e3f445726058a580540b34180b1d901bc6ad`  
		Last Modified: Thu, 23 Apr 2020 17:00:31 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d2907d69059834ae38df9cb5ce5abea2286c44944108ddc8df3b64d2072e3c`  
		Last Modified: Thu, 23 Apr 2020 17:00:42 GMT  
		Size: 24.8 MB (24793766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5639b6974ec6a0586ead06dbf648a68278de4759d13602db9a1829dc2cb25d75`  
		Last Modified: Thu, 23 Apr 2020 17:00:30 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39db0dc08d2fae5a5b6e0fb7f21074ba1438c9b266a6d744c8b6f8822e742bca`  
		Last Modified: Thu, 23 Apr 2020 17:00:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebcc61ca2620bd4f870fb0a74fdb77fcb9537c8db1fd17e40ab67a24ebc32e5`  
		Last Modified: Thu, 23 Apr 2020 17:00:30 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.2.4` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:d75f7d848405d07dea8af762cf052d029d05fc1ab3bb4d6bd42350b7af3f0808
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27145107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8037eab95b5e362188fb87562d495196b651ea499864f85b0e0945a5e907d26b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 09:24:49 GMT
ENV CONSUL_VERSION=1.2.4
# Fri, 24 Apr 2020 09:24:50 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 09:24:52 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 09:24:58 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 09:25:01 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 09:25:02 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 09:25:03 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 09:25:04 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 09:25:05 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 09:25:05 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 09:25:06 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 09:25:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:25:07 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9135996ebc8c26008490ea9eaeaf2d33a092ddb9b862addf499efb68255318d`  
		Last Modified: Fri, 24 Apr 2020 09:28:44 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d97bb3b4d363ddaf4744bf99247a774be1a9b2e2c23a21d4630d46825b6b4609`  
		Last Modified: Fri, 24 Apr 2020 09:28:52 GMT  
		Size: 24.4 MB (24447349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89eab74816070ac224055298a4354d0203ff72cde9ce635df82723ef700c9d49`  
		Last Modified: Fri, 24 Apr 2020 09:28:44 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301bd6c0ecfe81d7f5d130a8f8bc2214b721497c36fd9750a88ba4d07821c39a`  
		Last Modified: Fri, 24 Apr 2020 09:28:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc19ecd92f930789f56504c740bd2832784e2af968c57c8adcceea3a4478deee`  
		Last Modified: Fri, 24 Apr 2020 09:28:44 GMT  
		Size: 1.7 KB (1679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.2.4` - linux; 386

```console
$ docker pull consul@sha256:b9a93a22356863237ed47a3692f6e2fc40a5b0fa5e3d8b8c95f76ba507cdc9db
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28101751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e3e502fdb651377d03b343346bda8d434d8718463104359331977ee30ed7bbd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 04:31:40 GMT
ENV CONSUL_VERSION=1.2.4
# Fri, 24 Apr 2020 04:31:41 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 04:31:41 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 04:31:46 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 04:31:47 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 04:31:48 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 04:31:48 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 04:31:48 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 04:31:48 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 04:31:48 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 04:31:49 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 04:31:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:31:49 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cdc7080aa5cc8080f04d30e5771a15fbf5d8d6dd249e30fb0039e632a12c856`  
		Last Modified: Fri, 24 Apr 2020 04:33:30 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee895264375d68e371e42de8cdb7676ede8f2201c9d50f0a794d8cc7065eb56`  
		Last Modified: Fri, 24 Apr 2020 04:33:36 GMT  
		Size: 25.3 MB (25328787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b88d9a79f4beb250b040b661aa73be2a783b1b2c85e25577546c1187245ac3`  
		Last Modified: Fri, 24 Apr 2020 04:33:30 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e95e69b1d54b002d348a2c673da9bcc4688a23a90f0d8d91d8a584cd72bec7`  
		Last Modified: Fri, 24 Apr 2020 04:33:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddd71981e8a6865516e8d14d62639591c70baaee9bb2e595a73b30fca471616`  
		Last Modified: Fri, 24 Apr 2020 04:33:30 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.3`

```console
$ docker pull consul@sha256:6b76c55092a3daf5bb22e0085ef197a58c220b547a53ccd36392828b1271a831
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.3` - linux; amd64

```console
$ docker pull consul@sha256:d27562479ce549baa8da29ab7bdfa896fbe9b94134ea8729506923bd95037ed6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.6 MB (38571735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc9cce00996b86b7d64bb5f7d4c518772ade8ada160dc5c5a036eb9c3d0a297a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 14:18:04 GMT
ENV CONSUL_VERSION=1.3.1
# Fri, 24 Apr 2020 14:18:04 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 14:18:05 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 14:18:09 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 14:18:10 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 14:18:11 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:18:11 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 14:18:11 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 14:18:11 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 14:18:11 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 14:18:12 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:18:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:18:12 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc91ab599b3659dbd1c653e643cf44a432e64e26dce7746fcc45ec5a5432e714`  
		Last Modified: Fri, 24 Apr 2020 14:20:02 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b3e2647fcc7e9af911ccb1dfb7dc26630932aa19ee7ae16647eea1ae9b1334`  
		Last Modified: Fri, 24 Apr 2020 14:20:07 GMT  
		Size: 35.8 MB (35795092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fda538109b036f092eed83ebf5ade02c1d4015c23e717689c91bf66698cddea`  
		Last Modified: Fri, 24 Apr 2020 14:20:01 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1cfd8e14d735d0312bdeccc7c2280324700fa2b658aed73fdb9cf269e31c0e`  
		Last Modified: Fri, 24 Apr 2020 14:20:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9140b8996ba5142d2213b9f27e80e42e5ad633ae3557abfcaec6ab1f7418ac3b`  
		Last Modified: Fri, 24 Apr 2020 14:20:01 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.3` - linux; arm variant v6

```console
$ docker pull consul@sha256:4bc706953ad42c620d87e67bcc6816fa3d3a6e22f39056333816bec9aa7776c7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36396594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c24e4e72fa9e4b19c5fb8f63caf838628e8b9db75f2911aaf021bee6132872de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Apr 2020 16:55:28 GMT
ENV CONSUL_VERSION=1.3.1
# Thu, 23 Apr 2020 16:55:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Apr 2020 16:55:31 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Apr 2020 16:55:46 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Apr 2020 16:55:52 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Apr 2020 16:55:58 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 16:55:59 GMT
VOLUME [/consul/data]
# Thu, 23 Apr 2020 16:56:00 GMT
EXPOSE 8300
# Thu, 23 Apr 2020 16:56:02 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Apr 2020 16:56:03 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Apr 2020 16:56:04 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Apr 2020 16:56:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:56:07 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eb0dfd7e7346167838c1a76eec79673081440d7b0f96016cdd1b80419120ce`  
		Last Modified: Thu, 23 Apr 2020 17:00:06 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989235e8aafc3d56452784c31382fba7d60f9b1e4229e2943397a348cbb91e51`  
		Last Modified: Thu, 23 Apr 2020 17:00:19 GMT  
		Size: 33.8 MB (33844579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec087e98bcb596767137ea813be12c851540803b8c3e42d61cbb046fc7830fa`  
		Last Modified: Thu, 23 Apr 2020 17:00:06 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a9b94ae73012b59492f3fa8e1d7806fd04f7691e6a0064bf8dbd8edac7b6fc`  
		Last Modified: Thu, 23 Apr 2020 17:00:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb0c0e3165cdf269e929600f84320db083f7c296dcddbd701ce61cb9e980ee9`  
		Last Modified: Thu, 23 Apr 2020 17:00:06 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.3` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:015372d20892db2eb85a3fe52e64effa492c706a2d4b0c95c5abc1a6b0adc519
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36217726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a9a4a6be21baf6cf21dbf90ba59d36c6372c078ec271d86aee0db6672f6ce98`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 09:24:12 GMT
ENV CONSUL_VERSION=1.3.1
# Fri, 24 Apr 2020 09:24:12 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 09:24:14 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 09:24:20 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 09:24:23 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 09:24:25 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 09:24:26 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 09:24:27 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 09:24:28 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 09:24:30 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 09:24:31 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 09:24:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:24:33 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc89f0c84f920ded682a59ce2ffaed3eda996dd1d3a1c3e513adb4585836e65`  
		Last Modified: Fri, 24 Apr 2020 09:28:23 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c32847854933c7a96f4fb1c8e9020ca43f79feeae957c84c2ad1b628cf9f5d`  
		Last Modified: Fri, 24 Apr 2020 09:28:34 GMT  
		Size: 33.5 MB (33519971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e261f3f3eec08f2aa437229fd8c4485c941b2951cbe33981f1a2bd2ec264d5`  
		Last Modified: Fri, 24 Apr 2020 09:28:22 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c1e3e20cd62cf88aef402f6a184d54d9ff2b545b99e0fcc01fc145cd7b3472`  
		Last Modified: Fri, 24 Apr 2020 09:28:22 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ba016182a770579191b6719d3361c2e0d95ea9bbb2c28faef9c1d0f0c1a18b`  
		Last Modified: Fri, 24 Apr 2020 09:28:23 GMT  
		Size: 1.7 KB (1679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.3` - linux; 386

```console
$ docker pull consul@sha256:3f2640bd30e022b61ce7a9cf1660fc998fc5185355d23c44c73be440906bac16
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37754435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26a1f2d3dd5e0ca24dd18892ec8283293dc45db41fb32a073d4ac64a2430f710`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 04:31:28 GMT
ENV CONSUL_VERSION=1.3.1
# Fri, 24 Apr 2020 04:31:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 04:31:29 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 04:31:34 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 04:31:34 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 04:31:35 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 04:31:35 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 04:31:36 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 04:31:36 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 04:31:36 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 04:31:36 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 04:31:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:31:37 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1e9a4531a2d9978c118f72f554e90497f39bf1e9c4a3a96ded33d874076c61`  
		Last Modified: Fri, 24 Apr 2020 04:33:19 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4554f2aa7ab01b93d8c18cbdfee24588b194d763f19972138273ea2fd052d480`  
		Last Modified: Fri, 24 Apr 2020 04:33:25 GMT  
		Size: 35.0 MB (34981467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f81c8f14470667483b45dcedc54df4e89fd8d1a192d77ab918c34523a5d2f2f`  
		Last Modified: Fri, 24 Apr 2020 04:33:20 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51f091770b7dc5333f1f62ec308f1ccd4a895272fd521ffc3a78c712b578f25`  
		Last Modified: Fri, 24 Apr 2020 04:33:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7fdaec4321a4851d744f73e3241aabdf9292e9942fbf7f7bd457faac310c06`  
		Last Modified: Fri, 24 Apr 2020 04:33:19 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.3.1`

```console
$ docker pull consul@sha256:6b76c55092a3daf5bb22e0085ef197a58c220b547a53ccd36392828b1271a831
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.3.1` - linux; amd64

```console
$ docker pull consul@sha256:d27562479ce549baa8da29ab7bdfa896fbe9b94134ea8729506923bd95037ed6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.6 MB (38571735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc9cce00996b86b7d64bb5f7d4c518772ade8ada160dc5c5a036eb9c3d0a297a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 14:18:04 GMT
ENV CONSUL_VERSION=1.3.1
# Fri, 24 Apr 2020 14:18:04 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 14:18:05 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 14:18:09 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 14:18:10 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 14:18:11 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:18:11 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 14:18:11 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 14:18:11 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 14:18:11 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 14:18:12 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:18:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:18:12 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc91ab599b3659dbd1c653e643cf44a432e64e26dce7746fcc45ec5a5432e714`  
		Last Modified: Fri, 24 Apr 2020 14:20:02 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b3e2647fcc7e9af911ccb1dfb7dc26630932aa19ee7ae16647eea1ae9b1334`  
		Last Modified: Fri, 24 Apr 2020 14:20:07 GMT  
		Size: 35.8 MB (35795092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fda538109b036f092eed83ebf5ade02c1d4015c23e717689c91bf66698cddea`  
		Last Modified: Fri, 24 Apr 2020 14:20:01 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1cfd8e14d735d0312bdeccc7c2280324700fa2b658aed73fdb9cf269e31c0e`  
		Last Modified: Fri, 24 Apr 2020 14:20:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9140b8996ba5142d2213b9f27e80e42e5ad633ae3557abfcaec6ab1f7418ac3b`  
		Last Modified: Fri, 24 Apr 2020 14:20:01 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.3.1` - linux; arm variant v6

```console
$ docker pull consul@sha256:4bc706953ad42c620d87e67bcc6816fa3d3a6e22f39056333816bec9aa7776c7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36396594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c24e4e72fa9e4b19c5fb8f63caf838628e8b9db75f2911aaf021bee6132872de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Apr 2020 16:55:28 GMT
ENV CONSUL_VERSION=1.3.1
# Thu, 23 Apr 2020 16:55:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Apr 2020 16:55:31 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Apr 2020 16:55:46 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Apr 2020 16:55:52 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Apr 2020 16:55:58 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 16:55:59 GMT
VOLUME [/consul/data]
# Thu, 23 Apr 2020 16:56:00 GMT
EXPOSE 8300
# Thu, 23 Apr 2020 16:56:02 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Apr 2020 16:56:03 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Apr 2020 16:56:04 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Apr 2020 16:56:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:56:07 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eb0dfd7e7346167838c1a76eec79673081440d7b0f96016cdd1b80419120ce`  
		Last Modified: Thu, 23 Apr 2020 17:00:06 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989235e8aafc3d56452784c31382fba7d60f9b1e4229e2943397a348cbb91e51`  
		Last Modified: Thu, 23 Apr 2020 17:00:19 GMT  
		Size: 33.8 MB (33844579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec087e98bcb596767137ea813be12c851540803b8c3e42d61cbb046fc7830fa`  
		Last Modified: Thu, 23 Apr 2020 17:00:06 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a9b94ae73012b59492f3fa8e1d7806fd04f7691e6a0064bf8dbd8edac7b6fc`  
		Last Modified: Thu, 23 Apr 2020 17:00:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb0c0e3165cdf269e929600f84320db083f7c296dcddbd701ce61cb9e980ee9`  
		Last Modified: Thu, 23 Apr 2020 17:00:06 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.3.1` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:015372d20892db2eb85a3fe52e64effa492c706a2d4b0c95c5abc1a6b0adc519
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36217726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a9a4a6be21baf6cf21dbf90ba59d36c6372c078ec271d86aee0db6672f6ce98`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 09:24:12 GMT
ENV CONSUL_VERSION=1.3.1
# Fri, 24 Apr 2020 09:24:12 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 09:24:14 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 09:24:20 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 09:24:23 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 09:24:25 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 09:24:26 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 09:24:27 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 09:24:28 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 09:24:30 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 09:24:31 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 09:24:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:24:33 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc89f0c84f920ded682a59ce2ffaed3eda996dd1d3a1c3e513adb4585836e65`  
		Last Modified: Fri, 24 Apr 2020 09:28:23 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c32847854933c7a96f4fb1c8e9020ca43f79feeae957c84c2ad1b628cf9f5d`  
		Last Modified: Fri, 24 Apr 2020 09:28:34 GMT  
		Size: 33.5 MB (33519971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e261f3f3eec08f2aa437229fd8c4485c941b2951cbe33981f1a2bd2ec264d5`  
		Last Modified: Fri, 24 Apr 2020 09:28:22 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c1e3e20cd62cf88aef402f6a184d54d9ff2b545b99e0fcc01fc145cd7b3472`  
		Last Modified: Fri, 24 Apr 2020 09:28:22 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ba016182a770579191b6719d3361c2e0d95ea9bbb2c28faef9c1d0f0c1a18b`  
		Last Modified: Fri, 24 Apr 2020 09:28:23 GMT  
		Size: 1.7 KB (1679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.3.1` - linux; 386

```console
$ docker pull consul@sha256:3f2640bd30e022b61ce7a9cf1660fc998fc5185355d23c44c73be440906bac16
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37754435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26a1f2d3dd5e0ca24dd18892ec8283293dc45db41fb32a073d4ac64a2430f710`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 04:31:28 GMT
ENV CONSUL_VERSION=1.3.1
# Fri, 24 Apr 2020 04:31:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 04:31:29 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 04:31:34 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 04:31:34 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 04:31:35 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 04:31:35 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 04:31:36 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 04:31:36 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 04:31:36 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 04:31:36 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 04:31:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:31:37 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1e9a4531a2d9978c118f72f554e90497f39bf1e9c4a3a96ded33d874076c61`  
		Last Modified: Fri, 24 Apr 2020 04:33:19 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4554f2aa7ab01b93d8c18cbdfee24588b194d763f19972138273ea2fd052d480`  
		Last Modified: Fri, 24 Apr 2020 04:33:25 GMT  
		Size: 35.0 MB (34981467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f81c8f14470667483b45dcedc54df4e89fd8d1a192d77ab918c34523a5d2f2f`  
		Last Modified: Fri, 24 Apr 2020 04:33:20 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51f091770b7dc5333f1f62ec308f1ccd4a895272fd521ffc3a78c712b578f25`  
		Last Modified: Fri, 24 Apr 2020 04:33:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7fdaec4321a4851d744f73e3241aabdf9292e9942fbf7f7bd457faac310c06`  
		Last Modified: Fri, 24 Apr 2020 04:33:19 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.4`

```console
$ docker pull consul@sha256:9c6c566817408b71bf6f36b8e528c590fd21cb66722d1d57ae24645548a0152a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.4` - linux; amd64

```console
$ docker pull consul@sha256:834757e8ad29d5f8f9da7e090f0687c98c6db3faa6cb9647a8e77f342f3ec1a3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39208191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d8142aa10e20b3448aa9f4ecabf1786179cad35193574ec6c5fbc1c4a3d4d56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 14:17:52 GMT
ENV CONSUL_VERSION=1.4.5
# Fri, 24 Apr 2020 14:17:52 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 14:17:53 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 14:17:57 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 14:17:58 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 14:17:58 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:17:59 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 14:17:59 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 14:17:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 14:17:59 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 14:17:59 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:18:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:18:00 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c134567e0503761b8ce46d4101745ea73ca7989efdc24fa94be792154fa659a`  
		Last Modified: Fri, 24 Apr 2020 14:19:50 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4648b7e526ac5ef4bcdfe62765d24d879102be5d862cf21f0d29748cd485c0a6`  
		Last Modified: Fri, 24 Apr 2020 14:19:55 GMT  
		Size: 36.4 MB (36431550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c72e0e1211d55ce30c7776aa04831fb49e01f4c2a672291db55a76fe2182f063`  
		Last Modified: Fri, 24 Apr 2020 14:19:49 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a202a1fcb47dfe020727ef246b8f93833edc01b136a7bf6448fc70b678677b`  
		Last Modified: Fri, 24 Apr 2020 14:19:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec6849b09a8e4215337bc6f4f0957ee7980fce35da5eeb62a8bda6b57b77d2d`  
		Last Modified: Fri, 24 Apr 2020 14:19:50 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.4` - linux; arm variant v6

```console
$ docker pull consul@sha256:b46336852e3dbfc6455cdbc9f93ec6f106bd4ddaa683ea345f17afa10c39dc27
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36975963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b23daecfc8abc2af29f8313f7ecde84a78c6ab55449160103c2e9a5b0290957`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Apr 2020 16:55:01 GMT
ENV CONSUL_VERSION=1.4.5
# Thu, 23 Apr 2020 16:55:01 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Apr 2020 16:55:03 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Apr 2020 16:55:11 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Apr 2020 16:55:14 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Apr 2020 16:55:16 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 16:55:17 GMT
VOLUME [/consul/data]
# Thu, 23 Apr 2020 16:55:18 GMT
EXPOSE 8300
# Thu, 23 Apr 2020 16:55:18 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Apr 2020 16:55:19 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Apr 2020 16:55:19 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Apr 2020 16:55:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:55:21 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc6a2c1c9905f1c2e05293927bd4dca9b2ea4d887a292d6c383e99f16e98e15`  
		Last Modified: Thu, 23 Apr 2020 16:59:49 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c1169780ec696a64b499a35ca473a20f4a2eeb0b742e572c9d1c1183ad122f`  
		Last Modified: Thu, 23 Apr 2020 16:59:54 GMT  
		Size: 34.4 MB (34423949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5a1d631b6086463cbdcad0750c6fd5864c28576b34df2bc29a22f89669f836`  
		Last Modified: Thu, 23 Apr 2020 16:59:49 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4dc00e27cb34467f4575dbc7966a56be1aa3be4f75d686a49ec7d6a6acb9a49`  
		Last Modified: Thu, 23 Apr 2020 16:59:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b66a04b11afc36bbd5445117a1847f7b2093d02cb552802a4457cc9a311e83`  
		Last Modified: Thu, 23 Apr 2020 16:59:49 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.4` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:112d0204a41cf93c21f41fa36ca3f6cd65c065f5e7f411bf0ec265b2d30aca7c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36791571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:040e8c9595a8734d9a427a70c206f2a133621c8e9a82624e23edc4add1be2529`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 09:23:41 GMT
ENV CONSUL_VERSION=1.4.5
# Fri, 24 Apr 2020 09:23:42 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 09:23:45 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 09:23:51 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 09:23:54 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 09:23:57 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 09:23:58 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 09:23:59 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 09:23:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 09:24:01 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 09:24:01 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 09:24:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:24:04 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c493cda9603afc6e23b25505efd8e1e32da816db13e4da2e92f4ec9f0f0b5bf`  
		Last Modified: Fri, 24 Apr 2020 09:28:04 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509ec259a926c0c385c907d71fc3f65ffbfaadd945a9d25f936cffb750311e56`  
		Last Modified: Fri, 24 Apr 2020 09:28:13 GMT  
		Size: 34.1 MB (34093815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3daf41bf007d3a4d40d2b4bdf3fcd2fc1b7c767e87df6d1d739eeaa5a700c5`  
		Last Modified: Fri, 24 Apr 2020 09:28:05 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462a54ff3cd982a4987eb099f5f9af3842a072a6a1749c9130186d3680940bcd`  
		Last Modified: Fri, 24 Apr 2020 09:28:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca6fba1e121d0fae4ceea08c896e417cb2782800fd850b766c65ce9452965b98`  
		Last Modified: Fri, 24 Apr 2020 09:28:04 GMT  
		Size: 1.7 KB (1680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.4` - linux; 386

```console
$ docker pull consul@sha256:86423594c5d6c41564cba1f9d40e4326d67382d3b2f4aaa5e06a08e3289141ae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38368757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48f8b7990c7b5663a89f420f2bf180b0928be2fc0aa7f75c56d48a9cbc907bf2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 04:31:15 GMT
ENV CONSUL_VERSION=1.4.5
# Fri, 24 Apr 2020 04:31:16 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 04:31:16 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 04:31:21 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 04:31:22 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 04:31:23 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 04:31:23 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 04:31:23 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 04:31:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 04:31:24 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 04:31:24 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 04:31:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:31:24 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8b2b8200addb01a891e59e12456203f3628107edfd46fb6dc482da42fea289`  
		Last Modified: Fri, 24 Apr 2020 04:33:08 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f135280e1333dafa73df7d8473f7ee64f9c8f95d7c47b7b9dd152cd7f3770b05`  
		Last Modified: Fri, 24 Apr 2020 04:33:14 GMT  
		Size: 35.6 MB (35595790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9f6cc9c31ec9b55c5e894fd8717b29a969f109444e94167194b8e2dfaac0c7`  
		Last Modified: Fri, 24 Apr 2020 04:33:08 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85771b22dfb460e940cd0ae5bf5daaf56a177c1c1a161a69512c803e5c2eb9d`  
		Last Modified: Fri, 24 Apr 2020 04:33:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c599d350e76f776c8f981b6fa6d19dc1788d92a1a3f557d109a2ea0126bdcc`  
		Last Modified: Fri, 24 Apr 2020 04:33:08 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.4.5`

```console
$ docker pull consul@sha256:9c6c566817408b71bf6f36b8e528c590fd21cb66722d1d57ae24645548a0152a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.4.5` - linux; amd64

```console
$ docker pull consul@sha256:834757e8ad29d5f8f9da7e090f0687c98c6db3faa6cb9647a8e77f342f3ec1a3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39208191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d8142aa10e20b3448aa9f4ecabf1786179cad35193574ec6c5fbc1c4a3d4d56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 14:17:52 GMT
ENV CONSUL_VERSION=1.4.5
# Fri, 24 Apr 2020 14:17:52 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 14:17:53 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 14:17:57 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 14:17:58 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 14:17:58 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:17:59 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 14:17:59 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 14:17:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 14:17:59 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 14:17:59 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:18:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:18:00 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c134567e0503761b8ce46d4101745ea73ca7989efdc24fa94be792154fa659a`  
		Last Modified: Fri, 24 Apr 2020 14:19:50 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4648b7e526ac5ef4bcdfe62765d24d879102be5d862cf21f0d29748cd485c0a6`  
		Last Modified: Fri, 24 Apr 2020 14:19:55 GMT  
		Size: 36.4 MB (36431550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c72e0e1211d55ce30c7776aa04831fb49e01f4c2a672291db55a76fe2182f063`  
		Last Modified: Fri, 24 Apr 2020 14:19:49 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a202a1fcb47dfe020727ef246b8f93833edc01b136a7bf6448fc70b678677b`  
		Last Modified: Fri, 24 Apr 2020 14:19:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec6849b09a8e4215337bc6f4f0957ee7980fce35da5eeb62a8bda6b57b77d2d`  
		Last Modified: Fri, 24 Apr 2020 14:19:50 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.4.5` - linux; arm variant v6

```console
$ docker pull consul@sha256:b46336852e3dbfc6455cdbc9f93ec6f106bd4ddaa683ea345f17afa10c39dc27
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36975963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b23daecfc8abc2af29f8313f7ecde84a78c6ab55449160103c2e9a5b0290957`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Apr 2020 16:55:01 GMT
ENV CONSUL_VERSION=1.4.5
# Thu, 23 Apr 2020 16:55:01 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Apr 2020 16:55:03 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Apr 2020 16:55:11 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Apr 2020 16:55:14 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Apr 2020 16:55:16 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 16:55:17 GMT
VOLUME [/consul/data]
# Thu, 23 Apr 2020 16:55:18 GMT
EXPOSE 8300
# Thu, 23 Apr 2020 16:55:18 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Apr 2020 16:55:19 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Apr 2020 16:55:19 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Apr 2020 16:55:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:55:21 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc6a2c1c9905f1c2e05293927bd4dca9b2ea4d887a292d6c383e99f16e98e15`  
		Last Modified: Thu, 23 Apr 2020 16:59:49 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c1169780ec696a64b499a35ca473a20f4a2eeb0b742e572c9d1c1183ad122f`  
		Last Modified: Thu, 23 Apr 2020 16:59:54 GMT  
		Size: 34.4 MB (34423949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5a1d631b6086463cbdcad0750c6fd5864c28576b34df2bc29a22f89669f836`  
		Last Modified: Thu, 23 Apr 2020 16:59:49 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4dc00e27cb34467f4575dbc7966a56be1aa3be4f75d686a49ec7d6a6acb9a49`  
		Last Modified: Thu, 23 Apr 2020 16:59:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b66a04b11afc36bbd5445117a1847f7b2093d02cb552802a4457cc9a311e83`  
		Last Modified: Thu, 23 Apr 2020 16:59:49 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.4.5` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:112d0204a41cf93c21f41fa36ca3f6cd65c065f5e7f411bf0ec265b2d30aca7c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36791571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:040e8c9595a8734d9a427a70c206f2a133621c8e9a82624e23edc4add1be2529`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 09:23:41 GMT
ENV CONSUL_VERSION=1.4.5
# Fri, 24 Apr 2020 09:23:42 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 09:23:45 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 09:23:51 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 09:23:54 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 09:23:57 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 09:23:58 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 09:23:59 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 09:23:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 09:24:01 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 09:24:01 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 09:24:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:24:04 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c493cda9603afc6e23b25505efd8e1e32da816db13e4da2e92f4ec9f0f0b5bf`  
		Last Modified: Fri, 24 Apr 2020 09:28:04 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509ec259a926c0c385c907d71fc3f65ffbfaadd945a9d25f936cffb750311e56`  
		Last Modified: Fri, 24 Apr 2020 09:28:13 GMT  
		Size: 34.1 MB (34093815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3daf41bf007d3a4d40d2b4bdf3fcd2fc1b7c767e87df6d1d739eeaa5a700c5`  
		Last Modified: Fri, 24 Apr 2020 09:28:05 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462a54ff3cd982a4987eb099f5f9af3842a072a6a1749c9130186d3680940bcd`  
		Last Modified: Fri, 24 Apr 2020 09:28:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca6fba1e121d0fae4ceea08c896e417cb2782800fd850b766c65ce9452965b98`  
		Last Modified: Fri, 24 Apr 2020 09:28:04 GMT  
		Size: 1.7 KB (1680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.4.5` - linux; 386

```console
$ docker pull consul@sha256:86423594c5d6c41564cba1f9d40e4326d67382d3b2f4aaa5e06a08e3289141ae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38368757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48f8b7990c7b5663a89f420f2bf180b0928be2fc0aa7f75c56d48a9cbc907bf2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 04:31:15 GMT
ENV CONSUL_VERSION=1.4.5
# Fri, 24 Apr 2020 04:31:16 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 04:31:16 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 04:31:21 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 04:31:22 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 04:31:23 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 04:31:23 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 04:31:23 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 04:31:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 04:31:24 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 04:31:24 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 04:31:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:31:24 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8b2b8200addb01a891e59e12456203f3628107edfd46fb6dc482da42fea289`  
		Last Modified: Fri, 24 Apr 2020 04:33:08 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f135280e1333dafa73df7d8473f7ee64f9c8f95d7c47b7b9dd152cd7f3770b05`  
		Last Modified: Fri, 24 Apr 2020 04:33:14 GMT  
		Size: 35.6 MB (35595790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9f6cc9c31ec9b55c5e894fd8717b29a969f109444e94167194b8e2dfaac0c7`  
		Last Modified: Fri, 24 Apr 2020 04:33:08 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85771b22dfb460e940cd0ae5bf5daaf56a177c1c1a161a69512c803e5c2eb9d`  
		Last Modified: Fri, 24 Apr 2020 04:33:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c599d350e76f776c8f981b6fa6d19dc1788d92a1a3f557d109a2ea0126bdcc`  
		Last Modified: Fri, 24 Apr 2020 04:33:08 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.5`

```console
$ docker pull consul@sha256:0e7b52eecffb7e58c2395849b3e966b31fb9fe907e2c47b4aa83bc94591db2cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.5` - linux; amd64

```console
$ docker pull consul@sha256:9f3233b8e058d4396dc1a6b56451aa7ba3bccdd54e93f2cae9ea2dc65d1c84ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44190732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3ef0d4deb4b3a66a6670eefa68274c13d868414c8842b2baaaa1c871649081c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 14:17:40 GMT
ENV CONSUL_VERSION=1.5.3
# Fri, 24 Apr 2020 14:17:40 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 14:17:41 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 14:17:45 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 14:17:46 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 14:17:47 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:17:47 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 14:17:47 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 14:17:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 14:17:47 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 14:17:47 GMT
COPY file:1c5f16053db7ac80ca2606114b1597e5421edf31162ea24a1ae8b059f48426f0 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:17:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:17:48 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5736994e7cab6cd3d6cfe3b41581b2555527763007bec69cc1113d851d39b16`  
		Last Modified: Fri, 24 Apr 2020 14:19:36 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca65ac92302c8ffb12f101409cde3cb51d6fb63c81c45654571ddc9aa14c78a4`  
		Last Modified: Fri, 24 Apr 2020 14:19:42 GMT  
		Size: 41.4 MB (41414065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092243f303caaffbd447c3e0b8dcff85058cf781c413ba385d1ad952704b39bb`  
		Last Modified: Fri, 24 Apr 2020 14:19:36 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b7b60d823d05f33b215454dea89a73917b44fbaa61575206facad48b2823dc`  
		Last Modified: Fri, 24 Apr 2020 14:19:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1f8811b25f088d7639239a71940f3c4f983221ff92980ac6ac6c0ab5e4aca6`  
		Last Modified: Fri, 24 Apr 2020 14:19:36 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.5` - linux; arm variant v6

```console
$ docker pull consul@sha256:ff332dcbc1c975cf0e9f97b7cdc17628d86613ec97dd177ab8d910b7b52edaab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41568703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14709419af3bf1f0a49998d7b68286650003b784c886e1f0317cb01b2fffaed0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Apr 2020 16:54:25 GMT
ENV CONSUL_VERSION=1.5.3
# Thu, 23 Apr 2020 16:54:25 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Apr 2020 16:54:27 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Apr 2020 16:54:38 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Apr 2020 16:54:43 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Apr 2020 16:54:47 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 16:54:49 GMT
VOLUME [/consul/data]
# Thu, 23 Apr 2020 16:54:50 GMT
EXPOSE 8300
# Thu, 23 Apr 2020 16:54:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Apr 2020 16:54:52 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Apr 2020 16:54:53 GMT
COPY file:1c5f16053db7ac80ca2606114b1597e5421edf31162ea24a1ae8b059f48426f0 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Apr 2020 16:54:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:54:55 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828086b8d7d91f4c09cb0970444f1c9d4e21273a3c999ec514a666c74d92361d`  
		Last Modified: Thu, 23 Apr 2020 16:59:28 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5d7a670146edc486ef7717c5bc485a5fd43b1ef268b8573d83ce0d99eae508`  
		Last Modified: Thu, 23 Apr 2020 16:59:38 GMT  
		Size: 39.0 MB (39016662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d856f5478a381990258f8f0eccf2a569669ac03142d17ecaa855fe570b140a`  
		Last Modified: Thu, 23 Apr 2020 16:59:28 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19539467f60ea7c0deafae4c562165c8225b6046047b740a3d7446aa4005e322`  
		Last Modified: Thu, 23 Apr 2020 16:59:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9ed0d4d8a34d9590b1e5c97972755278a3b19ee99303dcc4c46c36c87f7a98`  
		Last Modified: Thu, 23 Apr 2020 16:59:28 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.5` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:8d0e289a510ab295e48ac3dfb030404c47c4ed248bf266cfa1e0697640da6157
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41737174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bec31d06062a1662db379771470d27a8d1eb3d6921dfee7f9e159b3bc7f5e191`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 09:23:17 GMT
ENV CONSUL_VERSION=1.5.3
# Fri, 24 Apr 2020 09:23:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 09:23:19 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 09:23:26 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 09:23:28 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 09:23:30 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 09:23:31 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 09:23:31 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 09:23:32 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 09:23:33 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 09:23:34 GMT
COPY file:1c5f16053db7ac80ca2606114b1597e5421edf31162ea24a1ae8b059f48426f0 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 09:23:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:23:35 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f253c4726e21ab12ddc6f1f8c0f7cc766afe44286638b8a3436f462b11704b2b`  
		Last Modified: Fri, 24 Apr 2020 09:27:36 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ccaaa96ac23a8d7d9a0f61c35c5fbc6be9df28059d154d33afd347178d8a79`  
		Last Modified: Fri, 24 Apr 2020 09:27:54 GMT  
		Size: 39.0 MB (39039393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518734cbd4fac105bf52f1749a8f050a7e7a0918a8cb97648a2251c028143862`  
		Last Modified: Fri, 24 Apr 2020 09:27:35 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e460b3dfa0f279d35031514869daca6c021e57be1496c86b74bf256d6ccf774`  
		Last Modified: Fri, 24 Apr 2020 09:27:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695f71e441fc67590d171b400754214617ab0ddc5825f4fb280cbc4e057b580d`  
		Last Modified: Fri, 24 Apr 2020 09:27:35 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.5` - linux; 386

```console
$ docker pull consul@sha256:6b984cc5dae695862a8d7b2a075e011d81f9b9b710d392c99845d902ff36bced
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43094688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78a6106b89ce5d052f34ccd0848d646e1bb0a3cca64488b2ebf2f65b534ceafb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 04:31:01 GMT
ENV CONSUL_VERSION=1.5.3
# Fri, 24 Apr 2020 04:31:02 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 04:31:02 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 04:31:08 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 04:31:08 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 04:31:09 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 04:31:09 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 04:31:10 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 04:31:10 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 04:31:10 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 04:31:10 GMT
COPY file:1c5f16053db7ac80ca2606114b1597e5421edf31162ea24a1ae8b059f48426f0 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 04:31:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:31:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3374db1f49fc2155d0d21f82a744d34851aa1e0e549d7e7f043e3106952a8c1e`  
		Last Modified: Fri, 24 Apr 2020 04:32:57 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a332ea3adc7dfdbb16bf9023e1ab94df85adaad801c06931061d599296df37e`  
		Last Modified: Fri, 24 Apr 2020 04:33:03 GMT  
		Size: 40.3 MB (40321693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118c0e8dc76e675fdc5b57fe37ea1bf62e5a14688cbf471324d5df068ca27cc0`  
		Last Modified: Fri, 24 Apr 2020 04:32:56 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2482ee4cfa303bdd919ed1245d7cefb6db230d741d24e7d335ea89f6fac9bc1`  
		Last Modified: Fri, 24 Apr 2020 04:32:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24266bee77a3f06e1448eda49f0b1a15ac0eae7bf313a82e55512d12b4b2b6e0`  
		Last Modified: Fri, 24 Apr 2020 04:32:56 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.5.3`

```console
$ docker pull consul@sha256:0e7b52eecffb7e58c2395849b3e966b31fb9fe907e2c47b4aa83bc94591db2cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.5.3` - linux; amd64

```console
$ docker pull consul@sha256:9f3233b8e058d4396dc1a6b56451aa7ba3bccdd54e93f2cae9ea2dc65d1c84ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44190732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3ef0d4deb4b3a66a6670eefa68274c13d868414c8842b2baaaa1c871649081c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 14:17:40 GMT
ENV CONSUL_VERSION=1.5.3
# Fri, 24 Apr 2020 14:17:40 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 14:17:41 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 14:17:45 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 14:17:46 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 14:17:47 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:17:47 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 14:17:47 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 14:17:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 14:17:47 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 14:17:47 GMT
COPY file:1c5f16053db7ac80ca2606114b1597e5421edf31162ea24a1ae8b059f48426f0 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:17:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:17:48 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5736994e7cab6cd3d6cfe3b41581b2555527763007bec69cc1113d851d39b16`  
		Last Modified: Fri, 24 Apr 2020 14:19:36 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca65ac92302c8ffb12f101409cde3cb51d6fb63c81c45654571ddc9aa14c78a4`  
		Last Modified: Fri, 24 Apr 2020 14:19:42 GMT  
		Size: 41.4 MB (41414065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092243f303caaffbd447c3e0b8dcff85058cf781c413ba385d1ad952704b39bb`  
		Last Modified: Fri, 24 Apr 2020 14:19:36 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b7b60d823d05f33b215454dea89a73917b44fbaa61575206facad48b2823dc`  
		Last Modified: Fri, 24 Apr 2020 14:19:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1f8811b25f088d7639239a71940f3c4f983221ff92980ac6ac6c0ab5e4aca6`  
		Last Modified: Fri, 24 Apr 2020 14:19:36 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.5.3` - linux; arm variant v6

```console
$ docker pull consul@sha256:ff332dcbc1c975cf0e9f97b7cdc17628d86613ec97dd177ab8d910b7b52edaab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41568703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14709419af3bf1f0a49998d7b68286650003b784c886e1f0317cb01b2fffaed0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Apr 2020 16:54:25 GMT
ENV CONSUL_VERSION=1.5.3
# Thu, 23 Apr 2020 16:54:25 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Apr 2020 16:54:27 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Apr 2020 16:54:38 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Apr 2020 16:54:43 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Apr 2020 16:54:47 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 16:54:49 GMT
VOLUME [/consul/data]
# Thu, 23 Apr 2020 16:54:50 GMT
EXPOSE 8300
# Thu, 23 Apr 2020 16:54:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Apr 2020 16:54:52 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Apr 2020 16:54:53 GMT
COPY file:1c5f16053db7ac80ca2606114b1597e5421edf31162ea24a1ae8b059f48426f0 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Apr 2020 16:54:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:54:55 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828086b8d7d91f4c09cb0970444f1c9d4e21273a3c999ec514a666c74d92361d`  
		Last Modified: Thu, 23 Apr 2020 16:59:28 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5d7a670146edc486ef7717c5bc485a5fd43b1ef268b8573d83ce0d99eae508`  
		Last Modified: Thu, 23 Apr 2020 16:59:38 GMT  
		Size: 39.0 MB (39016662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d856f5478a381990258f8f0eccf2a569669ac03142d17ecaa855fe570b140a`  
		Last Modified: Thu, 23 Apr 2020 16:59:28 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19539467f60ea7c0deafae4c562165c8225b6046047b740a3d7446aa4005e322`  
		Last Modified: Thu, 23 Apr 2020 16:59:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9ed0d4d8a34d9590b1e5c97972755278a3b19ee99303dcc4c46c36c87f7a98`  
		Last Modified: Thu, 23 Apr 2020 16:59:28 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.5.3` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:8d0e289a510ab295e48ac3dfb030404c47c4ed248bf266cfa1e0697640da6157
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41737174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bec31d06062a1662db379771470d27a8d1eb3d6921dfee7f9e159b3bc7f5e191`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 09:23:17 GMT
ENV CONSUL_VERSION=1.5.3
# Fri, 24 Apr 2020 09:23:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 09:23:19 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 09:23:26 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 09:23:28 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 09:23:30 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 09:23:31 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 09:23:31 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 09:23:32 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 09:23:33 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 09:23:34 GMT
COPY file:1c5f16053db7ac80ca2606114b1597e5421edf31162ea24a1ae8b059f48426f0 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 09:23:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:23:35 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f253c4726e21ab12ddc6f1f8c0f7cc766afe44286638b8a3436f462b11704b2b`  
		Last Modified: Fri, 24 Apr 2020 09:27:36 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ccaaa96ac23a8d7d9a0f61c35c5fbc6be9df28059d154d33afd347178d8a79`  
		Last Modified: Fri, 24 Apr 2020 09:27:54 GMT  
		Size: 39.0 MB (39039393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518734cbd4fac105bf52f1749a8f050a7e7a0918a8cb97648a2251c028143862`  
		Last Modified: Fri, 24 Apr 2020 09:27:35 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e460b3dfa0f279d35031514869daca6c021e57be1496c86b74bf256d6ccf774`  
		Last Modified: Fri, 24 Apr 2020 09:27:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695f71e441fc67590d171b400754214617ab0ddc5825f4fb280cbc4e057b580d`  
		Last Modified: Fri, 24 Apr 2020 09:27:35 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.5.3` - linux; 386

```console
$ docker pull consul@sha256:6b984cc5dae695862a8d7b2a075e011d81f9b9b710d392c99845d902ff36bced
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43094688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78a6106b89ce5d052f34ccd0848d646e1bb0a3cca64488b2ebf2f65b534ceafb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 04:31:01 GMT
ENV CONSUL_VERSION=1.5.3
# Fri, 24 Apr 2020 04:31:02 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 04:31:02 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 04:31:08 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 04:31:08 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 04:31:09 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 04:31:09 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 04:31:10 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 04:31:10 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 04:31:10 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 04:31:10 GMT
COPY file:1c5f16053db7ac80ca2606114b1597e5421edf31162ea24a1ae8b059f48426f0 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 04:31:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:31:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3374db1f49fc2155d0d21f82a744d34851aa1e0e549d7e7f043e3106952a8c1e`  
		Last Modified: Fri, 24 Apr 2020 04:32:57 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a332ea3adc7dfdbb16bf9023e1ab94df85adaad801c06931061d599296df37e`  
		Last Modified: Fri, 24 Apr 2020 04:33:03 GMT  
		Size: 40.3 MB (40321693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118c0e8dc76e675fdc5b57fe37ea1bf62e5a14688cbf471324d5df068ca27cc0`  
		Last Modified: Fri, 24 Apr 2020 04:32:56 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2482ee4cfa303bdd919ed1245d7cefb6db230d741d24e7d335ea89f6fac9bc1`  
		Last Modified: Fri, 24 Apr 2020 04:32:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24266bee77a3f06e1448eda49f0b1a15ac0eae7bf313a82e55512d12b4b2b6e0`  
		Last Modified: Fri, 24 Apr 2020 04:32:56 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.6`

```console
$ docker pull consul@sha256:fd819765a0562f49368aa79fb3cd56c8332024bd573d3d2eeb74bfea473d7b29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.6` - linux; amd64

```console
$ docker pull consul@sha256:739f316b4fe714ab38f8bc5d4c8db20e90dcc99e1a0140a7efe40a7e264be972
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.7 MB (44663330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f0739540c352e787b749b235f39c6ecb332c2891f5ccd76da3f23958b3a4527`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 14:17:27 GMT
ENV CONSUL_VERSION=1.6.4
# Fri, 24 Apr 2020 14:17:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 14:17:28 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 14:17:33 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 14:17:34 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 14:17:34 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:17:35 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 14:17:35 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 14:17:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 14:17:35 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 14:17:35 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:17:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:17:36 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1888a2146a605a9aa4b49f9263fe4fe97e0555c011f99e7d92117ddb691eb823`  
		Last Modified: Fri, 24 Apr 2020 14:19:21 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43d9e0e112d273351738855206c262226d0fa4ece78a9990ad40f249085c7e3`  
		Last Modified: Fri, 24 Apr 2020 14:19:27 GMT  
		Size: 41.9 MB (41886663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c8d962e6d1c5f276a8ce2592df9bacbe87eb0d10406a77f9c11beae134f12f`  
		Last Modified: Fri, 24 Apr 2020 14:19:21 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860768d967ce393cb995d47ca00deac3fa2dab24e7d25a4df1ca8409451e5409`  
		Last Modified: Fri, 24 Apr 2020 14:19:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e238d60eecae5a687e40ee823967976ec457e7db641ea06235b15063f4db76`  
		Last Modified: Fri, 24 Apr 2020 14:19:20 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; arm variant v6

```console
$ docker pull consul@sha256:ffde7f7119ba2b82be0cd46bc4a1b4b1046406c4541c2acee537a9eb594ee83d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (42041119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a961cfe68259a8f46766449996b547295ae12aaa5a8fea3f2ef4d1b304f169d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Apr 2020 16:53:53 GMT
ENV CONSUL_VERSION=1.6.4
# Thu, 23 Apr 2020 16:53:54 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Apr 2020 16:53:56 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Apr 2020 16:54:07 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Apr 2020 16:54:10 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Apr 2020 16:54:12 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 16:54:13 GMT
VOLUME [/consul/data]
# Thu, 23 Apr 2020 16:54:13 GMT
EXPOSE 8300
# Thu, 23 Apr 2020 16:54:14 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Apr 2020 16:54:15 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Apr 2020 16:54:15 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Apr 2020 16:54:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:54:17 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83c6e486bc251b948d2220b5138f16af3c90eafb66c61ddfb288ba9bc16c488`  
		Last Modified: Thu, 23 Apr 2020 16:59:11 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753852023b66df826ee77175e8071aceba91596dbb826636735502f592f5b7b2`  
		Last Modified: Thu, 23 Apr 2020 16:59:21 GMT  
		Size: 39.5 MB (39489079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171ce168cc0eec5045f16c757a6e195ee850a0c6fe5a35455eade5b7b21205b3`  
		Last Modified: Thu, 23 Apr 2020 16:59:11 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97521971145e342b2c6d92e6ad348d8ab8299fec5f5effe422e6a7dd66191b71`  
		Last Modified: Thu, 23 Apr 2020 16:59:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fdbe8131b8e1d3d21d683cf220bd62dc9acf2e1789eaa2c0748ce98ac0b358`  
		Last Modified: Thu, 23 Apr 2020 16:59:10 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:831349b601304201efdb523df7984152e4b23c85b68650a6557f0533ca3eb036
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40230722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:953c81b020c305ce1deacf33914ebea48c327e819871eec37164b102ae4430a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 09:22:53 GMT
ENV CONSUL_VERSION=1.6.4
# Fri, 24 Apr 2020 09:22:53 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 09:22:55 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 09:23:02 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 09:23:04 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 09:23:06 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 09:23:06 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 09:23:07 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 09:23:08 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 09:23:09 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 09:23:09 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 09:23:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:23:10 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87eeb6347257d448cdab813569ea0631b1efe2474d647010b4088c8218fe2ddc`  
		Last Modified: Fri, 24 Apr 2020 09:27:15 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f1ee7b2e79250128662a916072d34c63ce1bdb272a7ab4fc82db69aefc1f18`  
		Last Modified: Fri, 24 Apr 2020 09:27:26 GMT  
		Size: 37.5 MB (37532938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbd5c46008384e87907af51c381bac5355841b9836a1333eff4ec7f3842b236`  
		Last Modified: Fri, 24 Apr 2020 09:27:15 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2cfac48d21e57daadad080b41065a2256553a8280d85b01183e4496e92f3cd7`  
		Last Modified: Fri, 24 Apr 2020 09:27:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8518ed9911a980b9bb2244c47f27a3e605604e98b4818050748c36ff893343`  
		Last Modified: Fri, 24 Apr 2020 09:27:15 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; 386

```console
$ docker pull consul@sha256:a56cd17592810ef83c8b2cfea552e80ea1ff47e30a143e8dfd85f58d091edac0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.6 MB (43564854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e51ebb91e20f2ab0eab9b14934ace03d5c0c533dd2e65fddbbded72050ab651b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 04:30:47 GMT
ENV CONSUL_VERSION=1.6.4
# Fri, 24 Apr 2020 04:30:47 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 04:30:48 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 04:30:53 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 04:30:54 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 04:30:55 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 04:30:55 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 04:30:55 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 04:30:56 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 04:30:56 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 04:30:56 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 04:30:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:30:56 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f568d665eb8b0a76b0aa1413fda0d4420e3d26176df683dc9b5df735622a94`  
		Last Modified: Fri, 24 Apr 2020 04:32:45 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc8283ec022c872af08a5afbf7824fdb4f2250430a67afeb903c7ff57b33af9`  
		Last Modified: Fri, 24 Apr 2020 04:32:52 GMT  
		Size: 40.8 MB (40791861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a07385c2a70b08fb4573241222b0941b800763c74eb13ee946bdbcd89d0ec3c`  
		Last Modified: Fri, 24 Apr 2020 04:32:45 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3321e56ff68bad78adef6232b96a4cc1b2ea8b969e53ceb906ef71257982f195`  
		Last Modified: Fri, 24 Apr 2020 04:32:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6c76dbfbce3561478fe4a0afa0a544f01b73515f8bbbbb3b817774d1bd876a`  
		Last Modified: Fri, 24 Apr 2020 04:32:45 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.6.4`

```console
$ docker pull consul@sha256:fd819765a0562f49368aa79fb3cd56c8332024bd573d3d2eeb74bfea473d7b29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.6.4` - linux; amd64

```console
$ docker pull consul@sha256:739f316b4fe714ab38f8bc5d4c8db20e90dcc99e1a0140a7efe40a7e264be972
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.7 MB (44663330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f0739540c352e787b749b235f39c6ecb332c2891f5ccd76da3f23958b3a4527`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 14:17:27 GMT
ENV CONSUL_VERSION=1.6.4
# Fri, 24 Apr 2020 14:17:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 14:17:28 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 14:17:33 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 14:17:34 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 14:17:34 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:17:35 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 14:17:35 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 14:17:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 14:17:35 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 14:17:35 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:17:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:17:36 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1888a2146a605a9aa4b49f9263fe4fe97e0555c011f99e7d92117ddb691eb823`  
		Last Modified: Fri, 24 Apr 2020 14:19:21 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43d9e0e112d273351738855206c262226d0fa4ece78a9990ad40f249085c7e3`  
		Last Modified: Fri, 24 Apr 2020 14:19:27 GMT  
		Size: 41.9 MB (41886663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c8d962e6d1c5f276a8ce2592df9bacbe87eb0d10406a77f9c11beae134f12f`  
		Last Modified: Fri, 24 Apr 2020 14:19:21 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860768d967ce393cb995d47ca00deac3fa2dab24e7d25a4df1ca8409451e5409`  
		Last Modified: Fri, 24 Apr 2020 14:19:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e238d60eecae5a687e40ee823967976ec457e7db641ea06235b15063f4db76`  
		Last Modified: Fri, 24 Apr 2020 14:19:20 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6.4` - linux; arm variant v6

```console
$ docker pull consul@sha256:ffde7f7119ba2b82be0cd46bc4a1b4b1046406c4541c2acee537a9eb594ee83d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (42041119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a961cfe68259a8f46766449996b547295ae12aaa5a8fea3f2ef4d1b304f169d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Apr 2020 16:53:53 GMT
ENV CONSUL_VERSION=1.6.4
# Thu, 23 Apr 2020 16:53:54 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Apr 2020 16:53:56 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Apr 2020 16:54:07 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Apr 2020 16:54:10 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Apr 2020 16:54:12 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 16:54:13 GMT
VOLUME [/consul/data]
# Thu, 23 Apr 2020 16:54:13 GMT
EXPOSE 8300
# Thu, 23 Apr 2020 16:54:14 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Apr 2020 16:54:15 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Apr 2020 16:54:15 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Apr 2020 16:54:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:54:17 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83c6e486bc251b948d2220b5138f16af3c90eafb66c61ddfb288ba9bc16c488`  
		Last Modified: Thu, 23 Apr 2020 16:59:11 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753852023b66df826ee77175e8071aceba91596dbb826636735502f592f5b7b2`  
		Last Modified: Thu, 23 Apr 2020 16:59:21 GMT  
		Size: 39.5 MB (39489079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171ce168cc0eec5045f16c757a6e195ee850a0c6fe5a35455eade5b7b21205b3`  
		Last Modified: Thu, 23 Apr 2020 16:59:11 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97521971145e342b2c6d92e6ad348d8ab8299fec5f5effe422e6a7dd66191b71`  
		Last Modified: Thu, 23 Apr 2020 16:59:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fdbe8131b8e1d3d21d683cf220bd62dc9acf2e1789eaa2c0748ce98ac0b358`  
		Last Modified: Thu, 23 Apr 2020 16:59:10 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6.4` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:831349b601304201efdb523df7984152e4b23c85b68650a6557f0533ca3eb036
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40230722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:953c81b020c305ce1deacf33914ebea48c327e819871eec37164b102ae4430a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 09:22:53 GMT
ENV CONSUL_VERSION=1.6.4
# Fri, 24 Apr 2020 09:22:53 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 09:22:55 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 09:23:02 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 09:23:04 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 09:23:06 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 09:23:06 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 09:23:07 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 09:23:08 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 09:23:09 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 09:23:09 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 09:23:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:23:10 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87eeb6347257d448cdab813569ea0631b1efe2474d647010b4088c8218fe2ddc`  
		Last Modified: Fri, 24 Apr 2020 09:27:15 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f1ee7b2e79250128662a916072d34c63ce1bdb272a7ab4fc82db69aefc1f18`  
		Last Modified: Fri, 24 Apr 2020 09:27:26 GMT  
		Size: 37.5 MB (37532938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbd5c46008384e87907af51c381bac5355841b9836a1333eff4ec7f3842b236`  
		Last Modified: Fri, 24 Apr 2020 09:27:15 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2cfac48d21e57daadad080b41065a2256553a8280d85b01183e4496e92f3cd7`  
		Last Modified: Fri, 24 Apr 2020 09:27:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8518ed9911a980b9bb2244c47f27a3e605604e98b4818050748c36ff893343`  
		Last Modified: Fri, 24 Apr 2020 09:27:15 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6.4` - linux; 386

```console
$ docker pull consul@sha256:a56cd17592810ef83c8b2cfea552e80ea1ff47e30a143e8dfd85f58d091edac0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.6 MB (43564854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e51ebb91e20f2ab0eab9b14934ace03d5c0c533dd2e65fddbbded72050ab651b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 04:30:47 GMT
ENV CONSUL_VERSION=1.6.4
# Fri, 24 Apr 2020 04:30:47 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 04:30:48 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 04:30:53 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 04:30:54 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 04:30:55 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 04:30:55 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 04:30:55 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 04:30:56 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 04:30:56 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 04:30:56 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 04:30:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:30:56 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f568d665eb8b0a76b0aa1413fda0d4420e3d26176df683dc9b5df735622a94`  
		Last Modified: Fri, 24 Apr 2020 04:32:45 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc8283ec022c872af08a5afbf7824fdb4f2250430a67afeb903c7ff57b33af9`  
		Last Modified: Fri, 24 Apr 2020 04:32:52 GMT  
		Size: 40.8 MB (40791861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a07385c2a70b08fb4573241222b0941b800763c74eb13ee946bdbcd89d0ec3c`  
		Last Modified: Fri, 24 Apr 2020 04:32:45 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3321e56ff68bad78adef6232b96a4cc1b2ea8b969e53ceb906ef71257982f195`  
		Last Modified: Fri, 24 Apr 2020 04:32:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6c76dbfbce3561478fe4a0afa0a544f01b73515f8bbbbb3b817774d1bd876a`  
		Last Modified: Fri, 24 Apr 2020 04:32:45 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7`

```console
$ docker pull consul@sha256:4592d81f9cecdc9fe1832bdcd22dfceafd36720011539679ae177f62cf169ce6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7` - linux; amd64

```console
$ docker pull consul@sha256:7b29cb3aed7a314c3a9babbfc343448ac0795609443dc4e399ef9fd17b19c8b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (44039299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:197999eb696c8b907147bb108669c1a183e6683ceb6793c0a4e0d34e046959a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 14:17:15 GMT
ENV CONSUL_VERSION=1.7.2
# Fri, 24 Apr 2020 14:17:16 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 14:17:16 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 14:17:21 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 14:17:22 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 14:17:22 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:17:23 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 14:17:23 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 14:17:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 14:17:23 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 14:17:23 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:17:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:17:24 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1840596cea3b745a26f2464a9da90a282a7bf0f77fb43a5a876acf769517e081`  
		Last Modified: Fri, 24 Apr 2020 14:19:09 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce4a325e54a976ef5d60ef8fc60bf2c5c785fd5d95d022d604c76a53457261b`  
		Last Modified: Fri, 24 Apr 2020 14:19:15 GMT  
		Size: 41.3 MB (41262633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439a692865dcd828e7961f981acf0ec8527eadc09f263caddd3307023a64dda9`  
		Last Modified: Fri, 24 Apr 2020 14:19:08 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d6651b2ff51b4992b7e10ce284348acced7c0143cb9764e42516b5b066b7f5`  
		Last Modified: Fri, 24 Apr 2020 14:19:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0852833443ee3ab63680e2923807f97773e3ff6a2cb9e1859f2b6c90edc2df`  
		Last Modified: Fri, 24 Apr 2020 14:19:08 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm variant v6

```console
$ docker pull consul@sha256:2576c59acc486392580e50ded105e64b1978b932db016d9e90938b8e6d33d4b3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.4 MB (41373378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79208c31c835cd5fec058474d924af104bdeeb4b9d96f534a2ff1896b12e7ff4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Apr 2020 16:53:14 GMT
ENV CONSUL_VERSION=1.7.2
# Thu, 23 Apr 2020 16:53:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Apr 2020 16:53:17 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Apr 2020 16:53:38 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Apr 2020 16:53:40 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Apr 2020 16:53:42 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 16:53:43 GMT
VOLUME [/consul/data]
# Thu, 23 Apr 2020 16:53:43 GMT
EXPOSE 8300
# Thu, 23 Apr 2020 16:53:44 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Apr 2020 16:53:45 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Apr 2020 16:53:46 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Apr 2020 16:53:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:53:47 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9874fc1eb1d8751a0b682ebbc5d8c79d232643ec2a56f3b01f2fc7d1d0d2ebf2`  
		Last Modified: Thu, 23 Apr 2020 16:58:48 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564cdd5be6d3d2f6363923b22e5b77dcc12bf2b1bd669768afda1448739539c4`  
		Last Modified: Thu, 23 Apr 2020 16:59:02 GMT  
		Size: 38.8 MB (38821333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685d58b44180c7be022003e491ecd91499d30bf07744be7129d578aedef8315c`  
		Last Modified: Thu, 23 Apr 2020 16:58:48 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ac0ffd1df9fea7f273b6d0d2c4fe39c72b0734f71b4d228f3b8df05faf62da`  
		Last Modified: Thu, 23 Apr 2020 16:58:48 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2aef728bacc9219868ef13d7868146b3397a1a23089fc08e14751f2740a6cbf`  
		Last Modified: Thu, 23 Apr 2020 16:58:48 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:33f6cc6fe714d6879da71d6e254301ab74527a8ef5f042cfe9943d78bb34eb5d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41718052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2894ff433a6b082028a34580c4b6b3af69fa579a869e1fd67a9aac2f8a77dd3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 09:22:17 GMT
ENV CONSUL_VERSION=1.7.2
# Fri, 24 Apr 2020 09:22:19 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 09:22:23 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 09:22:33 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 09:22:36 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 09:22:38 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 09:22:39 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 09:22:39 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 09:22:40 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 09:22:41 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 09:22:41 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 09:22:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:22:43 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184e846a336b3bd958c312dc8f930f42bf56c7da5c64558248e6eaf9f0d6854b`  
		Last Modified: Fri, 24 Apr 2020 09:26:55 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca6cf198efa3d12bcb47c66fcba4285d0e9dbfe38d454d323223e97b9e90cf2`  
		Last Modified: Fri, 24 Apr 2020 09:27:04 GMT  
		Size: 39.0 MB (39020268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d783e033b4d46a91c3a484116ef6f25b25740a995aeb71c369635d50e6c01e92`  
		Last Modified: Fri, 24 Apr 2020 09:26:55 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a48e4cf4cfa4f52d9faaa1e94f66e3ffaae728422997ea03a7cad9c14254cdb`  
		Last Modified: Fri, 24 Apr 2020 09:26:55 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193477ec0e69c664d489bb8fbd415f5009dffcbafc6a7f9942eb31d504c695e8`  
		Last Modified: Fri, 24 Apr 2020 09:26:55 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; 386

```console
$ docker pull consul@sha256:392bdf13ef1354c14d04d1356edd45529424a37f05fed2fcdca5978ee4f4dba8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.8 MB (42801277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcde118126e62a34d36134d9f724ca494890204eac937d9ea6e74a3562fec002`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 04:30:33 GMT
ENV CONSUL_VERSION=1.7.2
# Fri, 24 Apr 2020 04:30:33 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 04:30:34 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 04:30:40 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 04:30:41 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 04:30:41 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 04:30:42 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 04:30:42 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 04:30:42 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 04:30:42 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 04:30:42 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 04:30:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:30:43 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607b7bb5061a95937d87f9ad985e42dacc435a6370d94152fc391ff32aa301be`  
		Last Modified: Fri, 24 Apr 2020 04:32:33 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa42f73ce141d946a080e2f0aefb7db4bbba77a41a6c4a264adc4e8d9520a2a2`  
		Last Modified: Fri, 24 Apr 2020 04:32:39 GMT  
		Size: 40.0 MB (40028283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d96e36abb3279217e16cf3ffcd6760567a8622deaf39a270c24d607e169d84`  
		Last Modified: Fri, 24 Apr 2020 04:32:32 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779aad3ecbda91cac2157b2d97bf8adc4f2b5bfd94304258f6e501bae7db49c3`  
		Last Modified: Fri, 24 Apr 2020 04:32:32 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38a902a831ce487125d829e4fe709443d1c1558ea81a5990448511187ea97d8`  
		Last Modified: Fri, 24 Apr 2020 04:32:33 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7.3`

```console
$ docker pull consul@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `consul:latest`

```console
$ docker pull consul@sha256:4592d81f9cecdc9fe1832bdcd22dfceafd36720011539679ae177f62cf169ce6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:7b29cb3aed7a314c3a9babbfc343448ac0795609443dc4e399ef9fd17b19c8b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (44039299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:197999eb696c8b907147bb108669c1a183e6683ceb6793c0a4e0d34e046959a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 14:17:15 GMT
ENV CONSUL_VERSION=1.7.2
# Fri, 24 Apr 2020 14:17:16 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 14:17:16 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 14:17:21 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 14:17:22 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 14:17:22 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:17:23 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 14:17:23 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 14:17:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 14:17:23 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 14:17:23 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:17:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:17:24 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1840596cea3b745a26f2464a9da90a282a7bf0f77fb43a5a876acf769517e081`  
		Last Modified: Fri, 24 Apr 2020 14:19:09 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce4a325e54a976ef5d60ef8fc60bf2c5c785fd5d95d022d604c76a53457261b`  
		Last Modified: Fri, 24 Apr 2020 14:19:15 GMT  
		Size: 41.3 MB (41262633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439a692865dcd828e7961f981acf0ec8527eadc09f263caddd3307023a64dda9`  
		Last Modified: Fri, 24 Apr 2020 14:19:08 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d6651b2ff51b4992b7e10ce284348acced7c0143cb9764e42516b5b066b7f5`  
		Last Modified: Fri, 24 Apr 2020 14:19:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0852833443ee3ab63680e2923807f97773e3ff6a2cb9e1859f2b6c90edc2df`  
		Last Modified: Fri, 24 Apr 2020 14:19:08 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:2576c59acc486392580e50ded105e64b1978b932db016d9e90938b8e6d33d4b3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.4 MB (41373378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79208c31c835cd5fec058474d924af104bdeeb4b9d96f534a2ff1896b12e7ff4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Apr 2020 16:53:14 GMT
ENV CONSUL_VERSION=1.7.2
# Thu, 23 Apr 2020 16:53:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Apr 2020 16:53:17 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Apr 2020 16:53:38 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Apr 2020 16:53:40 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Apr 2020 16:53:42 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 16:53:43 GMT
VOLUME [/consul/data]
# Thu, 23 Apr 2020 16:53:43 GMT
EXPOSE 8300
# Thu, 23 Apr 2020 16:53:44 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Apr 2020 16:53:45 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Apr 2020 16:53:46 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Apr 2020 16:53:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:53:47 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9874fc1eb1d8751a0b682ebbc5d8c79d232643ec2a56f3b01f2fc7d1d0d2ebf2`  
		Last Modified: Thu, 23 Apr 2020 16:58:48 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564cdd5be6d3d2f6363923b22e5b77dcc12bf2b1bd669768afda1448739539c4`  
		Last Modified: Thu, 23 Apr 2020 16:59:02 GMT  
		Size: 38.8 MB (38821333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685d58b44180c7be022003e491ecd91499d30bf07744be7129d578aedef8315c`  
		Last Modified: Thu, 23 Apr 2020 16:58:48 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ac0ffd1df9fea7f273b6d0d2c4fe39c72b0734f71b4d228f3b8df05faf62da`  
		Last Modified: Thu, 23 Apr 2020 16:58:48 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2aef728bacc9219868ef13d7868146b3397a1a23089fc08e14751f2740a6cbf`  
		Last Modified: Thu, 23 Apr 2020 16:58:48 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:33f6cc6fe714d6879da71d6e254301ab74527a8ef5f042cfe9943d78bb34eb5d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41718052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2894ff433a6b082028a34580c4b6b3af69fa579a869e1fd67a9aac2f8a77dd3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 09:22:17 GMT
ENV CONSUL_VERSION=1.7.2
# Fri, 24 Apr 2020 09:22:19 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 09:22:23 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 09:22:33 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 09:22:36 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 09:22:38 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 09:22:39 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 09:22:39 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 09:22:40 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 09:22:41 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 09:22:41 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 09:22:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:22:43 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184e846a336b3bd958c312dc8f930f42bf56c7da5c64558248e6eaf9f0d6854b`  
		Last Modified: Fri, 24 Apr 2020 09:26:55 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca6cf198efa3d12bcb47c66fcba4285d0e9dbfe38d454d323223e97b9e90cf2`  
		Last Modified: Fri, 24 Apr 2020 09:27:04 GMT  
		Size: 39.0 MB (39020268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d783e033b4d46a91c3a484116ef6f25b25740a995aeb71c369635d50e6c01e92`  
		Last Modified: Fri, 24 Apr 2020 09:26:55 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a48e4cf4cfa4f52d9faaa1e94f66e3ffaae728422997ea03a7cad9c14254cdb`  
		Last Modified: Fri, 24 Apr 2020 09:26:55 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193477ec0e69c664d489bb8fbd415f5009dffcbafc6a7f9942eb31d504c695e8`  
		Last Modified: Fri, 24 Apr 2020 09:26:55 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:392bdf13ef1354c14d04d1356edd45529424a37f05fed2fcdca5978ee4f4dba8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.8 MB (42801277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcde118126e62a34d36134d9f724ca494890204eac937d9ea6e74a3562fec002`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 24 Apr 2020 04:30:33 GMT
ENV CONSUL_VERSION=1.7.2
# Fri, 24 Apr 2020 04:30:33 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 24 Apr 2020 04:30:34 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 24 Apr 2020 04:30:40 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 24 Apr 2020 04:30:41 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 24 Apr 2020 04:30:41 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 04:30:42 GMT
VOLUME [/consul/data]
# Fri, 24 Apr 2020 04:30:42 GMT
EXPOSE 8300
# Fri, 24 Apr 2020 04:30:42 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 24 Apr 2020 04:30:42 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 24 Apr 2020 04:30:42 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 04:30:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:30:43 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607b7bb5061a95937d87f9ad985e42dacc435a6370d94152fc391ff32aa301be`  
		Last Modified: Fri, 24 Apr 2020 04:32:33 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa42f73ce141d946a080e2f0aefb7db4bbba77a41a6c4a264adc4e8d9520a2a2`  
		Last Modified: Fri, 24 Apr 2020 04:32:39 GMT  
		Size: 40.0 MB (40028283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d96e36abb3279217e16cf3ffcd6760567a8622deaf39a270c24d607e169d84`  
		Last Modified: Fri, 24 Apr 2020 04:32:32 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779aad3ecbda91cac2157b2d97bf8adc4f2b5bfd94304258f6e501bae7db49c3`  
		Last Modified: Fri, 24 Apr 2020 04:32:32 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38a902a831ce487125d829e4fe709443d1c1558ea81a5990448511187ea97d8`  
		Last Modified: Fri, 24 Apr 2020 04:32:33 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
