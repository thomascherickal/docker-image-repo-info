<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:1.2.6`](#vault126)
-	[`vault:1.3.9`](#vault139)
-	[`vault:1.4.5`](#vault145)
-	[`vault:1.5.2`](#vault152)
-	[`vault:latest`](#vaultlatest)

## `vault:1.2.6`

```console
$ docker pull vault@sha256:32453d07852a5c929b2cdb629fe2af99a8539b7f53b71e3a14470210fd29a9f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `vault:1.2.6` - linux; amd64

```console
$ docker pull vault@sha256:304ebd8fcc99defacc4590df9f0156dc5e930f52d428d252f9e2ea1376e5a339
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49442426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:079fd2299c06694404883455e5a5e14ed730b20a4a261937b086687518f740de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 21 Aug 2020 19:19:04 GMT
ARG VAULT_VERSION=1.2.6
# Fri, 21 Aug 2020 19:19:05 GMT
# ARGS: VAULT_VERSION=1.2.6
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 21 Aug 2020 19:19:12 GMT
# ARGS: VAULT_VERSION=1.2.6
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 21 Aug 2020 19:19:14 GMT
# ARGS: VAULT_VERSION=1.2.6
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 21 Aug 2020 19:19:14 GMT
VOLUME [/vault/logs]
# Fri, 21 Aug 2020 19:19:15 GMT
VOLUME [/vault/file]
# Fri, 21 Aug 2020 19:19:15 GMT
EXPOSE 8200
# Fri, 21 Aug 2020 19:19:15 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 21 Aug 2020 19:19:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Aug 2020 19:19:16 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49902ec9a569390219ff616b223a6176346fc84ba12b3b4b3772279a37df2eb0`  
		Last Modified: Fri, 21 Aug 2020 19:20:12 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2424ea86c828fb426d86b03b2d56a22f778c1da452747ea243104d4f9631c2a5`  
		Last Modified: Fri, 21 Aug 2020 19:20:22 GMT  
		Size: 46.6 MB (46643606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eff88841a2721b5ac7b5fd05df39d80e7b60404c26098da98c0ce8566863ab6`  
		Last Modified: Fri, 21 Aug 2020 19:20:12 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52278e1df399a98b8d05e48d6c00948058b59e165674a2c67ab4dcbc25060b4c`  
		Last Modified: Fri, 21 Aug 2020 19:20:12 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.2.6` - linux; arm variant v6

```console
$ docker pull vault@sha256:a27c9d23f4684cae4a96fa8ccefd14a9ef359e18d40a66e7e92ac69649e5f3a5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46537045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31185b73511096c51bbe9177859ea9eeb628b528dbb3f1d9f35c854e2559de0e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Fri, 21 Aug 2020 18:03:48 GMT
ARG VAULT_VERSION=1.2.6
# Fri, 21 Aug 2020 18:04:21 GMT
# ARGS: VAULT_VERSION=1.2.6
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 21 Aug 2020 18:04:59 GMT
# ARGS: VAULT_VERSION=1.2.6
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 21 Aug 2020 18:05:30 GMT
# ARGS: VAULT_VERSION=1.2.6
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 21 Aug 2020 18:05:36 GMT
VOLUME [/vault/logs]
# Fri, 21 Aug 2020 18:05:43 GMT
VOLUME [/vault/file]
# Fri, 21 Aug 2020 18:05:50 GMT
EXPOSE 8200
# Fri, 21 Aug 2020 18:06:03 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 21 Aug 2020 18:06:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Aug 2020 18:06:21 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3710d5164bdf6fb2b649cc62a3ca60b2f7367e7931c4a38c3d1f196cb0b1c5`  
		Last Modified: Fri, 21 Aug 2020 18:07:36 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bfe6db1c60fa2a2c8ca33fbb9be58f021aac53855c0ebe6737050275ea4525`  
		Last Modified: Fri, 21 Aug 2020 18:07:47 GMT  
		Size: 44.0 MB (43961230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74385b379901a95b903e0b50bae9a37fcb89e4e0fe267201a8d9ee0c45989c18`  
		Last Modified: Fri, 21 Aug 2020 18:07:35 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e494efa130628aeaca60b7d885fd0087e0fbfb7b8a6de2939a4885cef01d28`  
		Last Modified: Fri, 21 Aug 2020 18:07:35 GMT  
		Size: 1.8 KB (1826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.2.6` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:ea3150181fc5c5209d28fbfa002e93af2b8386659fc9c1e3e5251d4b479cb764
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.6 MB (46594724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:584093f3b3c0ebf9653eaec870bfbe240e2213d28a0a01e4fe900eacdd302e14`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 21 Aug 2020 19:09:41 GMT
ARG VAULT_VERSION=1.2.6
# Fri, 21 Aug 2020 19:09:43 GMT
# ARGS: VAULT_VERSION=1.2.6
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 21 Aug 2020 19:09:50 GMT
# ARGS: VAULT_VERSION=1.2.6
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 21 Aug 2020 19:09:52 GMT
# ARGS: VAULT_VERSION=1.2.6
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 21 Aug 2020 19:09:53 GMT
VOLUME [/vault/logs]
# Fri, 21 Aug 2020 19:09:54 GMT
VOLUME [/vault/file]
# Fri, 21 Aug 2020 19:09:54 GMT
EXPOSE 8200
# Fri, 21 Aug 2020 19:09:55 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 21 Aug 2020 19:09:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Aug 2020 19:09:56 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c206db4f771a175e4827e4375edef3470f86da39d4d46f25fcc8dbaf10ee23c8`  
		Last Modified: Fri, 21 Aug 2020 19:11:07 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489c7e7e125744316157199de2bac36fb28971ac03e380e19d2c3e276357cb55`  
		Last Modified: Fri, 21 Aug 2020 19:11:18 GMT  
		Size: 43.9 MB (43872691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0464b1468967478e599c6ceb5eb23fcdadefc3b4ee6fd4e5b5425b267e88fb`  
		Last Modified: Fri, 21 Aug 2020 19:11:07 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a99cfb28ef463d315a19fcb7fd28e2ccc0fde45df98e9796b072d179a82cc3`  
		Last Modified: Fri, 21 Aug 2020 19:11:07 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.3.9`

```console
$ docker pull vault@sha256:d5cfc46a41902be6d94f61091a9e986ae3374aafad57bfb5202ccf60b2df2e73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `vault:1.3.9` - linux; amd64

```console
$ docker pull vault@sha256:d22d8d06913aaa661fd59d39e63e789234f0a454c9c4f312a764e873974790de
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51664564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e0ea532086bc56fe718cdc288da4109409a3edbacca95e5129f6bbb1ea93f63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 21 Aug 2020 19:18:48 GMT
ARG VAULT_VERSION=1.3.9
# Fri, 21 Aug 2020 19:18:49 GMT
# ARGS: VAULT_VERSION=1.3.9
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 21 Aug 2020 19:18:55 GMT
# ARGS: VAULT_VERSION=1.3.9
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 21 Aug 2020 19:18:56 GMT
# ARGS: VAULT_VERSION=1.3.9
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 21 Aug 2020 19:18:57 GMT
VOLUME [/vault/logs]
# Fri, 21 Aug 2020 19:18:57 GMT
VOLUME [/vault/file]
# Fri, 21 Aug 2020 19:18:57 GMT
EXPOSE 8200
# Fri, 21 Aug 2020 19:18:58 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 21 Aug 2020 19:18:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Aug 2020 19:18:58 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba2a0e60e19196503f424ef1d2cf3effd679ed0af497f04d0438a13927ba23f`  
		Last Modified: Fri, 21 Aug 2020 19:19:57 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd332fa4ace9849777ec13be3d65b53f64f626d3605fbd799b563ac49fcf37e`  
		Last Modified: Fri, 21 Aug 2020 19:20:08 GMT  
		Size: 48.9 MB (48865745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7652a94f2671084ae7b48a65cc95bb46e5c2e132951ff0f26b77c37991f253c3`  
		Last Modified: Fri, 21 Aug 2020 19:19:57 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b281f08ae27609dde4c40cf15a37069393dc284e4056e119b1f14a9f63840c`  
		Last Modified: Fri, 21 Aug 2020 19:19:57 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.3.9` - linux; arm variant v6

```console
$ docker pull vault@sha256:e5ace478652e361d2515eca96c5fc36019b975fa1a308496ae3cdf1a526d3a6e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48656126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6aa929483b4d069b51b3582331c5322ecf188394ebc513e308ecb19f2374363`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Fri, 21 Aug 2020 18:00:15 GMT
ARG VAULT_VERSION=1.3.9
# Fri, 21 Aug 2020 18:00:52 GMT
# ARGS: VAULT_VERSION=1.3.9
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 21 Aug 2020 18:01:40 GMT
# ARGS: VAULT_VERSION=1.3.9
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 21 Aug 2020 18:02:21 GMT
# ARGS: VAULT_VERSION=1.3.9
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 21 Aug 2020 18:02:30 GMT
VOLUME [/vault/logs]
# Fri, 21 Aug 2020 18:02:36 GMT
VOLUME [/vault/file]
# Fri, 21 Aug 2020 18:02:42 GMT
EXPOSE 8200
# Fri, 21 Aug 2020 18:02:59 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 21 Aug 2020 18:03:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Aug 2020 18:03:22 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6fcb7880a621919f1759cc6eeda5dedde842706a1d0ffb5d5696383c4094853`  
		Last Modified: Fri, 21 Aug 2020 18:07:15 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24bbdc2d2280b70ca9e9ad968f9e0c1167706e09a28482eef19d94651f1ef0ae`  
		Last Modified: Fri, 21 Aug 2020 18:07:28 GMT  
		Size: 46.1 MB (46080313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51bd0d860baebf94bed1d0a9b8890f48c3320ef4a067b3fbad97d3a858fd4bf1`  
		Last Modified: Fri, 21 Aug 2020 18:07:15 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff92b13724d85e931973702bd08bc5ede26b436695ca246d47114bacc3457d8`  
		Last Modified: Fri, 21 Aug 2020 18:07:15 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.3.9` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:6c26f66fd25daefc176e0ea26444e7312c58351a08d7b7526ee3f7cf4dd63d1e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48695051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc5806c91f50af6ec53350ffa6e8ff6728ca6ec9f737705e716b561b0af1916d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 21 Aug 2020 19:09:20 GMT
ARG VAULT_VERSION=1.3.9
# Fri, 21 Aug 2020 19:09:21 GMT
# ARGS: VAULT_VERSION=1.3.9
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 21 Aug 2020 19:09:28 GMT
# ARGS: VAULT_VERSION=1.3.9
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 21 Aug 2020 19:09:31 GMT
# ARGS: VAULT_VERSION=1.3.9
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 21 Aug 2020 19:09:31 GMT
VOLUME [/vault/logs]
# Fri, 21 Aug 2020 19:09:32 GMT
VOLUME [/vault/file]
# Fri, 21 Aug 2020 19:09:33 GMT
EXPOSE 8200
# Fri, 21 Aug 2020 19:09:33 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 21 Aug 2020 19:09:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Aug 2020 19:09:35 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b432cc8d8402094e259da21932b7d8f2c2f7f085143bcc97dde64a6b70a5268f`  
		Last Modified: Fri, 21 Aug 2020 19:10:48 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e909eb488093a02ad05430eb50a09a0c77194f7775bffce05c8943b15fbaeb`  
		Last Modified: Fri, 21 Aug 2020 19:11:00 GMT  
		Size: 46.0 MB (45973015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e59e5a87c741c74a52dd69c74141608f2e2827e44cadbbf70e1b91b92ffc39a`  
		Last Modified: Fri, 21 Aug 2020 19:10:48 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3efe41e01c9ac49825b11f01b982d7ff5478aad9d57682887047da2324b146ed`  
		Last Modified: Fri, 21 Aug 2020 19:10:48 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.4.5`

```console
$ docker pull vault@sha256:c48a5b3125b2a25cebcb51c0446cde7dcd466f2e24e4833bb5377f34c4dc8263
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `vault:1.4.5` - linux; amd64

```console
$ docker pull vault@sha256:1da3c2159dfb3d867542fe514d673c043ae5517c9d58f135ee19b60f3210fb92
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52072246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd9d838e3e5aab754ff4049f401c6e1b919a30fa86cf555f4c9febf439636ea7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 21 Aug 2020 19:18:29 GMT
ARG VAULT_VERSION=1.4.5
# Fri, 21 Aug 2020 19:18:31 GMT
# ARGS: VAULT_VERSION=1.4.5
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 21 Aug 2020 19:18:38 GMT
# ARGS: VAULT_VERSION=1.4.5
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 21 Aug 2020 19:18:40 GMT
# ARGS: VAULT_VERSION=1.4.5
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 21 Aug 2020 19:18:40 GMT
VOLUME [/vault/logs]
# Fri, 21 Aug 2020 19:18:40 GMT
VOLUME [/vault/file]
# Fri, 21 Aug 2020 19:18:40 GMT
EXPOSE 8200
# Fri, 21 Aug 2020 19:18:41 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 21 Aug 2020 19:18:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Aug 2020 19:18:41 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e73ea30dda0c5ec0ec230dd9ca1b348be422fa18ffb6641b22c7806bdc2afcd`  
		Last Modified: Fri, 21 Aug 2020 19:19:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924c5df630351a37172e39935d5c8d1d5e0ac89313839580e48f680253990dd6`  
		Last Modified: Fri, 21 Aug 2020 19:19:54 GMT  
		Size: 49.3 MB (49273431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d475e2154a492c3d2d363204aa139e19934bc730d6d023373ab7a903b5ead`  
		Last Modified: Fri, 21 Aug 2020 19:19:43 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc9215c7277d0747853694fffecb65a41f6167b12f0a55a75fe8eb031086d61`  
		Last Modified: Fri, 21 Aug 2020 19:19:44 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.4.5` - linux; arm variant v6

```console
$ docker pull vault@sha256:1ea20650a103ad8c9008f01ac0d48d5ba94fc6add3371e91c9765fd323d13f87
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48715199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1d8fb5e33b5b4548c8fdb84d0d5b55d08afc561b2b144c7b6eefdf2c484b816`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Fri, 21 Aug 2020 17:56:49 GMT
ARG VAULT_VERSION=1.4.5
# Fri, 21 Aug 2020 17:57:17 GMT
# ARGS: VAULT_VERSION=1.4.5
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 21 Aug 2020 17:58:03 GMT
# ARGS: VAULT_VERSION=1.4.5
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 21 Aug 2020 17:58:44 GMT
# ARGS: VAULT_VERSION=1.4.5
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 21 Aug 2020 17:58:54 GMT
VOLUME [/vault/logs]
# Fri, 21 Aug 2020 17:59:00 GMT
VOLUME [/vault/file]
# Fri, 21 Aug 2020 17:59:10 GMT
EXPOSE 8200
# Fri, 21 Aug 2020 17:59:27 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 21 Aug 2020 17:59:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Aug 2020 17:59:45 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95b854c6dd2b2f51cbe01e3a4a5cff3eea6351bf4dcd01509f6a136fe94b890`  
		Last Modified: Fri, 21 Aug 2020 18:06:55 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:887a049ac803026f1b467005bb09fd146d9675382594d327bbdb0de755d28971`  
		Last Modified: Fri, 21 Aug 2020 18:07:08 GMT  
		Size: 46.1 MB (46139387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e982690aa4706be10447be1d91bd6844e83d5854d2f7dd4c1a7d344d0b600851`  
		Last Modified: Fri, 21 Aug 2020 18:06:55 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98c320d4b9215d15c6362d43047218a9fbb6804ac0bf62b5317e487dbdeb223`  
		Last Modified: Fri, 21 Aug 2020 18:06:55 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.4.5` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:957d6e942313e760d3004fdd82ab48967808e72cf2ef23d671e15f4cf41a9dcb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48951758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:056080bd2f94932beb4472fd0d18bd23584bfdb568f562b5d3e13fff3b178bb1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 21 Aug 2020 19:08:56 GMT
ARG VAULT_VERSION=1.4.5
# Fri, 21 Aug 2020 19:08:58 GMT
# ARGS: VAULT_VERSION=1.4.5
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 21 Aug 2020 19:09:05 GMT
# ARGS: VAULT_VERSION=1.4.5
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 21 Aug 2020 19:09:07 GMT
# ARGS: VAULT_VERSION=1.4.5
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 21 Aug 2020 19:09:08 GMT
VOLUME [/vault/logs]
# Fri, 21 Aug 2020 19:09:09 GMT
VOLUME [/vault/file]
# Fri, 21 Aug 2020 19:09:09 GMT
EXPOSE 8200
# Fri, 21 Aug 2020 19:09:10 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 21 Aug 2020 19:09:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Aug 2020 19:09:11 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4499595616267f4c8b2ed83c857750ccea3359cabbe201988b2f4a9cfd45fb7`  
		Last Modified: Fri, 21 Aug 2020 19:10:30 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a38067711a4c8f7744f57f5e650c87d2bfaf4842d6ddaf2b8cd85ccd7d5f172`  
		Last Modified: Fri, 21 Aug 2020 19:10:42 GMT  
		Size: 46.2 MB (46229725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a9cc5c2fdada9e8439a07cf72d3e1c3469f0267661a3052a9612ad1918883e`  
		Last Modified: Fri, 21 Aug 2020 19:10:30 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb9bb54d0eca43cda34a7379000bf39f1894a619da0d734fc2cc5191093d5cc`  
		Last Modified: Fri, 21 Aug 2020 19:10:31 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.5.2`

```console
$ docker pull vault@sha256:61cddb923f2cc579b55cbf072d8714e470fc34a4ff828fda23c89d821044399f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `vault:1.5.2` - linux; amd64

```console
$ docker pull vault@sha256:d8e230e3995e6a58349d90c40393c5e6c33a35d419dca31e5b2f11e5f26c210c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55001916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14889d38c67545d7b96c510e816782c52426c3e8545af34d7c2ffa792c151ee1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 21 Aug 2020 19:18:10 GMT
ARG VAULT_VERSION=1.5.2
# Fri, 21 Aug 2020 19:18:11 GMT
# ARGS: VAULT_VERSION=1.5.2
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 21 Aug 2020 19:18:20 GMT
# ARGS: VAULT_VERSION=1.5.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 21 Aug 2020 19:18:21 GMT
# ARGS: VAULT_VERSION=1.5.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 21 Aug 2020 19:18:22 GMT
VOLUME [/vault/logs]
# Fri, 21 Aug 2020 19:18:22 GMT
VOLUME [/vault/file]
# Fri, 21 Aug 2020 19:18:22 GMT
EXPOSE 8200
# Fri, 21 Aug 2020 19:18:23 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 21 Aug 2020 19:18:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Aug 2020 19:18:23 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3b7e4276dd5ad9c3dfaaf1424dba7a6f15a4e09df2266c92da6d97a182e418`  
		Last Modified: Fri, 21 Aug 2020 19:19:29 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c904ae0f10cfe3d473dd76ad2829bfb30a81a1534e84289499623faa33b8a72`  
		Last Modified: Fri, 21 Aug 2020 19:19:39 GMT  
		Size: 52.2 MB (52203100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351356674c870478218f981698fd3ad4fa991e6b1b8b510bc154c7ac6c4ba27d`  
		Last Modified: Fri, 21 Aug 2020 19:19:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7780ab5359928ed984cdc8a18654804dfbba80b0b7e227f066d515adff2451d`  
		Last Modified: Fri, 21 Aug 2020 19:19:28 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.5.2` - linux; arm variant v6

```console
$ docker pull vault@sha256:7509003ece487d0ac4df08d5bd7875f4fe97234ec819f91c288056f084c62fa7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51550076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f74a680705453c2fa1ed1e484bd4d7e18f4154efb9c4b531bee5f16b3674c9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Fri, 21 Aug 2020 17:54:15 GMT
ARG VAULT_VERSION=1.5.2
# Fri, 21 Aug 2020 17:54:42 GMT
# ARGS: VAULT_VERSION=1.5.2
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 21 Aug 2020 17:55:21 GMT
# ARGS: VAULT_VERSION=1.5.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 21 Aug 2020 17:55:49 GMT
# ARGS: VAULT_VERSION=1.5.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 21 Aug 2020 17:55:55 GMT
VOLUME [/vault/logs]
# Fri, 21 Aug 2020 17:56:01 GMT
VOLUME [/vault/file]
# Fri, 21 Aug 2020 17:56:07 GMT
EXPOSE 8200
# Fri, 21 Aug 2020 17:56:18 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 21 Aug 2020 17:56:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Aug 2020 17:56:30 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc6abc070bd5f5861e48c418ceac66274d409f1de73c78e209a121bbd1551d7`  
		Last Modified: Fri, 21 Aug 2020 18:06:33 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09dd3f6bdd6fa6c4641034644f1eb16fd2f64e03c9ac9c66e2dbc345d98727a6`  
		Last Modified: Fri, 21 Aug 2020 18:06:46 GMT  
		Size: 49.0 MB (48974263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a023f876d8d7dcbb63a69c0eed38fe28fc8ce32b28ecbfbe51eca4569833071`  
		Last Modified: Fri, 21 Aug 2020 18:06:33 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0ef6bbd727f6920d99b321848bfbddde0c56f4371265a48656fb05c05569e2`  
		Last Modified: Fri, 21 Aug 2020 18:06:33 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.5.2` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:4e072c7e7622579e0e463f668563b23d046afaf28950cf3475221a91e76ac618
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51919116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc20548ad12b95cadb9be7e532d5649cae92d8c50371e4cbeda23a8db14bbedb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 21 Aug 2020 19:08:29 GMT
ARG VAULT_VERSION=1.5.2
# Fri, 21 Aug 2020 19:08:31 GMT
# ARGS: VAULT_VERSION=1.5.2
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 21 Aug 2020 19:08:41 GMT
# ARGS: VAULT_VERSION=1.5.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 21 Aug 2020 19:08:43 GMT
# ARGS: VAULT_VERSION=1.5.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 21 Aug 2020 19:08:44 GMT
VOLUME [/vault/logs]
# Fri, 21 Aug 2020 19:08:45 GMT
VOLUME [/vault/file]
# Fri, 21 Aug 2020 19:08:45 GMT
EXPOSE 8200
# Fri, 21 Aug 2020 19:08:46 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 21 Aug 2020 19:08:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Aug 2020 19:08:47 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2e2a3a90170cf2a14df612f2bd9747f95704d1426bb44b84fe1f79de2396fc`  
		Last Modified: Fri, 21 Aug 2020 19:10:09 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcd1768948320328901c1ddea860c0380579c9d041b9373a3cfd681f1a6b62d`  
		Last Modified: Fri, 21 Aug 2020 19:10:23 GMT  
		Size: 49.2 MB (49197084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ca790cba5393f67ac47c17330a9ac419599eab0532d20487c96a9a1376a6a7`  
		Last Modified: Fri, 21 Aug 2020 19:10:09 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86179d02812454a6f52b196ff08e39fdb3ed42bd5b8bba49f9946973efbe4c7c`  
		Last Modified: Fri, 21 Aug 2020 19:10:09 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:latest`

```console
$ docker pull vault@sha256:6fc3a117ce9fea9041fa575cb0f02c4bf19aa4b3d97ce71ea3c8caba76084e2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:d8e230e3995e6a58349d90c40393c5e6c33a35d419dca31e5b2f11e5f26c210c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55001916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14889d38c67545d7b96c510e816782c52426c3e8545af34d7c2ffa792c151ee1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 21 Aug 2020 19:18:10 GMT
ARG VAULT_VERSION=1.5.2
# Fri, 21 Aug 2020 19:18:11 GMT
# ARGS: VAULT_VERSION=1.5.2
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 21 Aug 2020 19:18:20 GMT
# ARGS: VAULT_VERSION=1.5.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 21 Aug 2020 19:18:21 GMT
# ARGS: VAULT_VERSION=1.5.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 21 Aug 2020 19:18:22 GMT
VOLUME [/vault/logs]
# Fri, 21 Aug 2020 19:18:22 GMT
VOLUME [/vault/file]
# Fri, 21 Aug 2020 19:18:22 GMT
EXPOSE 8200
# Fri, 21 Aug 2020 19:18:23 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 21 Aug 2020 19:18:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Aug 2020 19:18:23 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3b7e4276dd5ad9c3dfaaf1424dba7a6f15a4e09df2266c92da6d97a182e418`  
		Last Modified: Fri, 21 Aug 2020 19:19:29 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c904ae0f10cfe3d473dd76ad2829bfb30a81a1534e84289499623faa33b8a72`  
		Last Modified: Fri, 21 Aug 2020 19:19:39 GMT  
		Size: 52.2 MB (52203100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351356674c870478218f981698fd3ad4fa991e6b1b8b510bc154c7ac6c4ba27d`  
		Last Modified: Fri, 21 Aug 2020 19:19:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7780ab5359928ed984cdc8a18654804dfbba80b0b7e227f066d515adff2451d`  
		Last Modified: Fri, 21 Aug 2020 19:19:28 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:7509003ece487d0ac4df08d5bd7875f4fe97234ec819f91c288056f084c62fa7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51550076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f74a680705453c2fa1ed1e484bd4d7e18f4154efb9c4b531bee5f16b3674c9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Fri, 21 Aug 2020 17:54:15 GMT
ARG VAULT_VERSION=1.5.2
# Fri, 21 Aug 2020 17:54:42 GMT
# ARGS: VAULT_VERSION=1.5.2
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 21 Aug 2020 17:55:21 GMT
# ARGS: VAULT_VERSION=1.5.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 21 Aug 2020 17:55:49 GMT
# ARGS: VAULT_VERSION=1.5.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 21 Aug 2020 17:55:55 GMT
VOLUME [/vault/logs]
# Fri, 21 Aug 2020 17:56:01 GMT
VOLUME [/vault/file]
# Fri, 21 Aug 2020 17:56:07 GMT
EXPOSE 8200
# Fri, 21 Aug 2020 17:56:18 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 21 Aug 2020 17:56:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Aug 2020 17:56:30 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc6abc070bd5f5861e48c418ceac66274d409f1de73c78e209a121bbd1551d7`  
		Last Modified: Fri, 21 Aug 2020 18:06:33 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09dd3f6bdd6fa6c4641034644f1eb16fd2f64e03c9ac9c66e2dbc345d98727a6`  
		Last Modified: Fri, 21 Aug 2020 18:06:46 GMT  
		Size: 49.0 MB (48974263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a023f876d8d7dcbb63a69c0eed38fe28fc8ce32b28ecbfbe51eca4569833071`  
		Last Modified: Fri, 21 Aug 2020 18:06:33 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0ef6bbd727f6920d99b321848bfbddde0c56f4371265a48656fb05c05569e2`  
		Last Modified: Fri, 21 Aug 2020 18:06:33 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:4e072c7e7622579e0e463f668563b23d046afaf28950cf3475221a91e76ac618
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51919116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc20548ad12b95cadb9be7e532d5649cae92d8c50371e4cbeda23a8db14bbedb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 21 Aug 2020 19:08:29 GMT
ARG VAULT_VERSION=1.5.2
# Fri, 21 Aug 2020 19:08:31 GMT
# ARGS: VAULT_VERSION=1.5.2
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 21 Aug 2020 19:08:41 GMT
# ARGS: VAULT_VERSION=1.5.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 21 Aug 2020 19:08:43 GMT
# ARGS: VAULT_VERSION=1.5.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 21 Aug 2020 19:08:44 GMT
VOLUME [/vault/logs]
# Fri, 21 Aug 2020 19:08:45 GMT
VOLUME [/vault/file]
# Fri, 21 Aug 2020 19:08:45 GMT
EXPOSE 8200
# Fri, 21 Aug 2020 19:08:46 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 21 Aug 2020 19:08:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Aug 2020 19:08:47 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2e2a3a90170cf2a14df612f2bd9747f95704d1426bb44b84fe1f79de2396fc`  
		Last Modified: Fri, 21 Aug 2020 19:10:09 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcd1768948320328901c1ddea860c0380579c9d041b9373a3cfd681f1a6b62d`  
		Last Modified: Fri, 21 Aug 2020 19:10:23 GMT  
		Size: 49.2 MB (49197084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ca790cba5393f67ac47c17330a9ac419599eab0532d20487c96a9a1376a6a7`  
		Last Modified: Fri, 21 Aug 2020 19:10:09 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86179d02812454a6f52b196ff08e39fdb3ed42bd5b8bba49f9946973efbe4c7c`  
		Last Modified: Fri, 21 Aug 2020 19:10:09 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:73e6d355c750f7ea852533734fead354d69c2526639e5978ac55e25e1f02a6d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52448518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02d5d0f6b760ba955d94c40e784ac2f01a3657755c0b61371571b0c53a2cf0ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Wed, 22 Jul 2020 02:20:52 GMT
ARG VAULT_VERSION=1.5.0
# Wed, 22 Jul 2020 02:20:53 GMT
# ARGS: VAULT_VERSION=1.5.0
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Jul 2020 02:21:00 GMT
# ARGS: VAULT_VERSION=1.5.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Jul 2020 02:21:00 GMT
# ARGS: VAULT_VERSION=1.5.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Jul 2020 02:21:01 GMT
VOLUME [/vault/logs]
# Wed, 22 Jul 2020 02:21:01 GMT
VOLUME [/vault/file]
# Wed, 22 Jul 2020 02:21:01 GMT
EXPOSE 8200
# Wed, 22 Jul 2020 02:21:01 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Jul 2020 02:21:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 02:21:02 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa6a4c14afcfefd047fd4c94647e87826f05c4a990e16fb2d7ba7b7bf1af2b5`  
		Last Modified: Wed, 22 Jul 2020 02:21:09 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3c4d290c2c65c69f7eae170d528203af72fc61e444f563b797f1907a556bcc`  
		Last Modified: Wed, 22 Jul 2020 02:21:18 GMT  
		Size: 49.7 MB (49658153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264fe782cf6cf4084484d38b675307e796bfaea00d8a3a66575500a82e586dbe`  
		Last Modified: Wed, 22 Jul 2020 02:21:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f27b55f8608662f53633b5036672f840dd1615868ada5247152bbff82f1cfe`  
		Last Modified: Wed, 22 Jul 2020 02:21:09 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
