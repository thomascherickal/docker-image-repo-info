## `vault:latest`

```console
$ docker pull vault@sha256:927cf913d9be6f16796b3c430ed0777debb38b90c156495ac250f2e27580ceed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:b8c73943dd14c56dda07500274232daca304d34598ed2cdbe0b6919bce9d72e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.0 MB (52034384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bc624ef8f0a2a776206c7a189711e344d94e998762ed43f477957849665b5d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Wed, 08 Apr 2020 22:27:58 GMT
ARG VAULT_VERSION=1.4.0
# Wed, 08 Apr 2020 22:27:59 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 08 Apr 2020 22:28:07 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 08 Apr 2020 22:28:09 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 08 Apr 2020 22:28:10 GMT
VOLUME [/vault/logs]
# Wed, 08 Apr 2020 22:28:10 GMT
VOLUME [/vault/file]
# Wed, 08 Apr 2020 22:28:10 GMT
EXPOSE 8200
# Wed, 08 Apr 2020 22:28:11 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 08 Apr 2020 22:28:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Apr 2020 22:28:11 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede16796b1954739ce0681c6b79999511c0f2092557def019fc115c2ceac0631`  
		Last Modified: Wed, 08 Apr 2020 22:28:22 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b639718572623b6344d84dbc1f35afd96133c37cf2646837e7b55159dac8f3d`  
		Last Modified: Wed, 08 Apr 2020 22:28:35 GMT  
		Size: 49.2 MB (49244187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99a4863f730d76a43274f73237d4c6eccd575480ef4848b6b902f912fc20441`  
		Last Modified: Wed, 08 Apr 2020 22:28:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45563f338d8e33f7c6c51613737a4e7d713f2de002942adc076b784f96270de0`  
		Last Modified: Wed, 08 Apr 2020 22:28:22 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:1684c860ff0aa5efba5723f1f0dadc709aa3a1732118d84f37450103d846eca1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48691759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eddd6978048d080a8a029c781f5b0a651f66a49011cc5ae5d8202b0837e44702`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 23:59:22 GMT
ARG VAULT_VERSION=1.4.0
# Thu, 23 Apr 2020 23:59:28 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 23 Apr 2020 23:59:48 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 23 Apr 2020 23:59:52 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 23 Apr 2020 23:59:53 GMT
VOLUME [/vault/logs]
# Thu, 23 Apr 2020 23:59:54 GMT
VOLUME [/vault/file]
# Thu, 23 Apr 2020 23:59:55 GMT
EXPOSE 8200
# Thu, 23 Apr 2020 23:59:55 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Apr 2020 23:59:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 23:59:57 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac68d33839fa5b66075f0433602084959d5077f9f3410c1068c7016bc3b5666`  
		Last Modified: Fri, 24 Apr 2020 00:00:13 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe1f661133ed03a53c5ed8bf8c946ee93acc665ba2c8a60e76486072ff456bf`  
		Last Modified: Fri, 24 Apr 2020 00:00:22 GMT  
		Size: 46.1 MB (46115952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bfe6fb0c8e8bf42dd1b6e6319f48d31d98188f5f12c2b115449426108cc758e`  
		Last Modified: Fri, 24 Apr 2020 00:00:12 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cce4fc8ec509f52a3bc38feb06438c37ad67ad39f3856b5678987633b47647a`  
		Last Modified: Fri, 24 Apr 2020 00:00:12 GMT  
		Size: 1.8 KB (1818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:8c9f07a6e75e529fdc5afaff8ed27474b23d2a711e3bfc01917c30a6b59e90f1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48958857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:522c11e9272057a0c2490d9ae46864673c6336274226efc06777509b16d8f22b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Wed, 08 Apr 2020 22:29:09 GMT
ARG VAULT_VERSION=1.4.0
# Wed, 08 Apr 2020 22:29:11 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 08 Apr 2020 22:29:20 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 08 Apr 2020 22:29:23 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 08 Apr 2020 22:29:24 GMT
VOLUME [/vault/logs]
# Wed, 08 Apr 2020 22:29:25 GMT
VOLUME [/vault/file]
# Wed, 08 Apr 2020 22:29:30 GMT
EXPOSE 8200
# Wed, 08 Apr 2020 22:29:31 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 08 Apr 2020 22:29:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Apr 2020 22:29:33 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a3480952c7b49ce97b6b7f6b0251d1da3fd7206c90155607b63dc658f79ffd`  
		Last Modified: Wed, 08 Apr 2020 22:29:45 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04839f2022d441841d6f48314cb0c30e3b65b0f2158d7a215de9c7a80003f3a5`  
		Last Modified: Wed, 08 Apr 2020 22:30:05 GMT  
		Size: 46.2 MB (46237828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504f8ea148642822355d44e57365c134e01b29307da7cc9704f698663dbcc8c9`  
		Last Modified: Wed, 08 Apr 2020 22:29:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c9404df0a3a7269e605d01aaf52cfe7df9ef500478f84ae2c8a195a17e4dd3`  
		Last Modified: Wed, 08 Apr 2020 22:29:45 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:e6ebca95ca196529950d784981ed4e33f70b041f03b993068e9aadb37214864e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50191547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:679c25688f13d33caff2d6e13de43136d78e5fb3c59fe9e7f9f0e243dde54c1f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:57 GMT
ADD file:8c429ecc11f3cadcecc39922ce15df6b51a649929959b331fed8d1f42d722474 in / 
# Thu, 23 Jan 2020 16:52:57 GMT
CMD ["/bin/sh"]
# Wed, 08 Apr 2020 23:33:02 GMT
ARG VAULT_VERSION=1.4.0
# Wed, 08 Apr 2020 23:33:03 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 08 Apr 2020 23:33:09 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 08 Apr 2020 23:33:09 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 08 Apr 2020 23:33:10 GMT
VOLUME [/vault/logs]
# Wed, 08 Apr 2020 23:33:10 GMT
VOLUME [/vault/file]
# Wed, 08 Apr 2020 23:33:10 GMT
EXPOSE 8200
# Wed, 08 Apr 2020 23:33:10 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 08 Apr 2020 23:33:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Apr 2020 23:33:11 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:8ad089020f8a1fd366fb13feb183e2f4c7410e2232c54b40f6a54fd56029fdf3`  
		Last Modified: Thu, 23 Jan 2020 16:53:22 GMT  
		Size: 2.8 MB (2785861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33885abdd7f1a2779259ded2b3490fb7ce6aeab36f62d94e08f6b6454c1950a`  
		Last Modified: Wed, 08 Apr 2020 23:33:19 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20643048ca305b027ac643c304101d13633e4802a7203d2479dce142446d60d`  
		Last Modified: Wed, 08 Apr 2020 23:33:28 GMT  
		Size: 47.4 MB (47402450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cd579fb11cc4fc8b8bd86bb1d5e60f509485ed1f618a2a09c0252a9137acaa`  
		Last Modified: Wed, 08 Apr 2020 23:33:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52b6bfc19bee65860faabbe36edd43db3d57421abe6eedbdb933320afacc671`  
		Last Modified: Wed, 08 Apr 2020 23:33:18 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
