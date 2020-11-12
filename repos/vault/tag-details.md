<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:1.4.7`](#vault147)
-	[`vault:1.5.5`](#vault155)
-	[`vault:1.6.0`](#vault160)
-	[`vault:latest`](#vaultlatest)

## `vault:1.4.7`

```console
$ docker pull vault@sha256:f9d13b0daa3dda2e606b3b08d0bfb4fc182896dc18c9e5f299e779c482e82b21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.4.7` - linux; amd64

```console
$ docker pull vault@sha256:dcd6dd72df4d702298c1867c6b35cbdb6c2baed157b93eeb2fa4a1cddf537387
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52077220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4975a63281100a1b5913581eca8216aeb630b404218b18b5e8d1fba0959aefa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 25 Sep 2020 22:23:56 GMT
ARG VAULT_VERSION=1.4.7
# Fri, 25 Sep 2020 22:23:56 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 25 Sep 2020 22:24:01 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 25 Sep 2020 22:24:02 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 25 Sep 2020 22:24:02 GMT
VOLUME [/vault/logs]
# Fri, 25 Sep 2020 22:24:03 GMT
VOLUME [/vault/file]
# Fri, 25 Sep 2020 22:24:03 GMT
EXPOSE 8200
# Fri, 25 Sep 2020 22:24:03 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 25 Sep 2020 22:24:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 22:24:03 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fbad820b6719fae861764d4019f1e52aa0fe755606258d837732859bdd74bc3`  
		Last Modified: Fri, 25 Sep 2020 22:24:26 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab03e04bd4c729386612e6521d19f92d92ad92dad9403ab40ea13e655039afb8`  
		Last Modified: Fri, 25 Sep 2020 22:24:35 GMT  
		Size: 49.3 MB (49278408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefa1a65e329cae9f864506f0bf3a8c5b1451475c597001ade81e7e21c6e63b9`  
		Last Modified: Fri, 25 Sep 2020 22:24:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862448950ddfb48fe80bd3f650eafd152bd5995059ead5928aea0af99e4a88ff`  
		Last Modified: Fri, 25 Sep 2020 22:24:26 GMT  
		Size: 1.8 KB (1818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.4.7` - linux; arm variant v6

```console
$ docker pull vault@sha256:58bf4fa10d4cbf8cffa451be7208a68a13403bfb49ae3bc26a5ddb1b64b8a272
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48714475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:448fd985b34d1da789a3c9f15bcbf2b01b1d95f4a3882d740ea2f4a61daeb918`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Fri, 25 Sep 2020 20:56:28 GMT
ARG VAULT_VERSION=1.4.7
# Fri, 25 Sep 2020 20:56:30 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 25 Sep 2020 20:56:39 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 25 Sep 2020 20:56:42 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 25 Sep 2020 20:56:42 GMT
VOLUME [/vault/logs]
# Fri, 25 Sep 2020 20:56:43 GMT
VOLUME [/vault/file]
# Fri, 25 Sep 2020 20:56:44 GMT
EXPOSE 8200
# Fri, 25 Sep 2020 20:56:44 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 25 Sep 2020 20:56:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 20:56:46 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116010314be70ee210793d5bd7e9cf6db6b93ca880e0dd374c120df5d16246eb`  
		Last Modified: Fri, 25 Sep 2020 20:57:16 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04698403a8d794c829e18563f1d28c0581206fb22a200e7076545fd76775bc7`  
		Last Modified: Fri, 25 Sep 2020 20:57:28 GMT  
		Size: 46.1 MB (46138660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6fc88ea91b5c5ce7c717fb34669f26426967e053abccea8b82c57f090897a18`  
		Last Modified: Fri, 25 Sep 2020 20:57:16 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e16c1fcf148c943608a6a20125e60127cb0f799ec370b27cc6de9a3a49d9588`  
		Last Modified: Fri, 25 Sep 2020 20:57:16 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.4.7` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:fff1e5df6f6366034edcf17d5a3047bb3fcbb2fc452f75afa5b98d479baa95a6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48959728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:606d48fcb08d8ccb45bb1dd553d4e66deae493966c3405cc1c96c969a30d07cc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 25 Sep 2020 21:02:08 GMT
ARG VAULT_VERSION=1.4.7
# Fri, 25 Sep 2020 21:02:10 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 25 Sep 2020 21:02:20 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 25 Sep 2020 21:02:23 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 25 Sep 2020 21:02:24 GMT
VOLUME [/vault/logs]
# Fri, 25 Sep 2020 21:02:25 GMT
VOLUME [/vault/file]
# Fri, 25 Sep 2020 21:02:26 GMT
EXPOSE 8200
# Fri, 25 Sep 2020 21:02:26 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 25 Sep 2020 21:02:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 21:02:28 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940df1224b1f0e4ea1c41d623b3cf2843512750c0df95f7ebfbc8db0a8f8f275`  
		Last Modified: Fri, 25 Sep 2020 21:03:03 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb53e464e5fc9b69fd7b0a5dbd46880ab8f099990266c46449337b66802865d1`  
		Last Modified: Fri, 25 Sep 2020 21:03:17 GMT  
		Size: 46.2 MB (46237693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0bbaa8186a2b81237c4e508485c1fc9f34bad5e5d7c09c9283528f0e90a246`  
		Last Modified: Fri, 25 Sep 2020 21:03:03 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c666812947b0131c0fd111c35c93e0ac898c824fc8a6f5f42eef564e6cc014b`  
		Last Modified: Fri, 25 Sep 2020 21:03:03 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.4.7` - linux; 386

```console
$ docker pull vault@sha256:b1ddef25ae7ce79858ca36f9dcc3bbd80fa19503dc08ebf693df0e41fb89cb16
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50210274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff0c5f6deb44c0e3ddfe53b0c289d2e175304eb8d78b10b9976af7952d56d4c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Fri, 25 Sep 2020 20:46:43 GMT
ARG VAULT_VERSION=1.4.7
# Fri, 25 Sep 2020 20:46:44 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 25 Sep 2020 20:46:49 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 25 Sep 2020 20:46:50 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 25 Sep 2020 20:46:50 GMT
VOLUME [/vault/logs]
# Fri, 25 Sep 2020 20:46:51 GMT
VOLUME [/vault/file]
# Fri, 25 Sep 2020 20:46:51 GMT
EXPOSE 8200
# Fri, 25 Sep 2020 20:46:51 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 25 Sep 2020 20:46:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 20:46:51 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af43af0d728f368be98762fdb7591feed512a62d95af452698644f90462b0258`  
		Last Modified: Fri, 25 Sep 2020 20:47:12 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe8d50ba1601a09ec5ee75b5de4e0f6c32160bb3da2ca09f890d240484b7ac0`  
		Last Modified: Fri, 25 Sep 2020 20:47:20 GMT  
		Size: 47.4 MB (47419912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f9a32f322b9ea82f698982bfd0b13205dfb564c81316759f662c230c531406`  
		Last Modified: Fri, 25 Sep 2020 20:47:12 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b7be61385badda541d9c962fb924b65feeaad92527cf56333704422c2be99a`  
		Last Modified: Fri, 25 Sep 2020 20:47:12 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.5.5`

```console
$ docker pull vault@sha256:a9ffb7244bc804897ca83e912cdd3bcc90392dd45a04d4d977d03584738a57d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.5.5` - linux; amd64

```console
$ docker pull vault@sha256:a5b242b5e16bda3a0584017fae2c589d344333074464013d9d3a19053c3843a6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54883751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00008a71f7a87913367e182031143ba2c746d4c14fac4b54e0b50bec8baadd98`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Tue, 27 Oct 2020 18:39:42 GMT
ARG VAULT_VERSION=1.5.5
# Tue, 27 Oct 2020 18:39:43 GMT
# ARGS: VAULT_VERSION=1.5.5
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 27 Oct 2020 18:39:48 GMT
# ARGS: VAULT_VERSION=1.5.5
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 27 Oct 2020 18:39:49 GMT
# ARGS: VAULT_VERSION=1.5.5
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 27 Oct 2020 18:39:49 GMT
VOLUME [/vault/logs]
# Tue, 27 Oct 2020 18:39:49 GMT
VOLUME [/vault/file]
# Tue, 27 Oct 2020 18:39:49 GMT
EXPOSE 8200
# Tue, 27 Oct 2020 18:39:50 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 27 Oct 2020 18:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:39:50 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdadead44d92de5777a4d869ccbfbcfa65e195673161d32969e2681d0a7119dd`  
		Last Modified: Tue, 27 Oct 2020 18:40:02 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d75306ea8d5906d76f9c00891367e1452175e046f9573659a7fc48d5b80b57a`  
		Last Modified: Tue, 27 Oct 2020 18:40:10 GMT  
		Size: 52.1 MB (52084928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f43b6cf66fd7c54b638ab490357caf5c1264361df0fdb713f2d40033073a3c`  
		Last Modified: Tue, 27 Oct 2020 18:40:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21738dc1af308babf352dd214f41c6b69b6dbba082801f3417288e3e8fe5cedd`  
		Last Modified: Tue, 27 Oct 2020 18:40:03 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.5.5` - linux; arm variant v6

```console
$ docker pull vault@sha256:7f6ba72d76f404bc72fca967703e2e3f78f366ba9e84e69b1082927b94ef131a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.4 MB (51434136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0535139ff4d58f921e848809a18abf675609ee5ca27f7eb64c97af4fcb6b6861`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Tue, 27 Oct 2020 18:52:16 GMT
ARG VAULT_VERSION=1.5.5
# Tue, 27 Oct 2020 18:52:17 GMT
# ARGS: VAULT_VERSION=1.5.5
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 27 Oct 2020 18:52:27 GMT
# ARGS: VAULT_VERSION=1.5.5
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 27 Oct 2020 18:52:30 GMT
# ARGS: VAULT_VERSION=1.5.5
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 27 Oct 2020 18:52:30 GMT
VOLUME [/vault/logs]
# Tue, 27 Oct 2020 18:52:31 GMT
VOLUME [/vault/file]
# Tue, 27 Oct 2020 18:52:31 GMT
EXPOSE 8200
# Tue, 27 Oct 2020 18:52:32 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 27 Oct 2020 18:52:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:52:33 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4407f73904898cf48c171bb591129cf76d4f25f1718cd3cef7e73304514e6cc`  
		Last Modified: Tue, 27 Oct 2020 18:52:48 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:394237de9a3fe23d190ffd8816664808787bb3b3fa002e04b42337b637d0cc7d`  
		Last Modified: Tue, 27 Oct 2020 18:53:01 GMT  
		Size: 48.9 MB (48858326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c196f608eab6bc1a1269473d9805e3f9d5124a3c968abd18106c82ab238a3a5d`  
		Last Modified: Tue, 27 Oct 2020 18:52:47 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:701418518cc6f035a94a27e2212464945b89e4b6d2ed2f162a9a214266d7aefd`  
		Last Modified: Tue, 27 Oct 2020 18:52:47 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.5.5` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:957fae6fc189f0021f760c8e1a5884b1f281a53767f90dd918ec6cbafee81985
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51779023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:321fa80e986836c996830367f76dfed5effb82027a6ad899a89909d55833c02d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Tue, 27 Oct 2020 18:41:23 GMT
ARG VAULT_VERSION=1.5.5
# Tue, 27 Oct 2020 18:41:25 GMT
# ARGS: VAULT_VERSION=1.5.5
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 27 Oct 2020 18:41:32 GMT
# ARGS: VAULT_VERSION=1.5.5
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 27 Oct 2020 18:41:35 GMT
# ARGS: VAULT_VERSION=1.5.5
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 27 Oct 2020 18:41:36 GMT
VOLUME [/vault/logs]
# Tue, 27 Oct 2020 18:41:36 GMT
VOLUME [/vault/file]
# Tue, 27 Oct 2020 18:41:37 GMT
EXPOSE 8200
# Tue, 27 Oct 2020 18:41:37 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 27 Oct 2020 18:41:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:41:39 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d447c612897e7927b4944767862ad58e31b57cc998c9fedc492c4be58ce0d4`  
		Last Modified: Tue, 27 Oct 2020 18:41:55 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f95b994568d39057958ca151c1c5efadec7da41f1b6d1c2e994539d62d86b8`  
		Last Modified: Tue, 27 Oct 2020 18:42:07 GMT  
		Size: 49.1 MB (49056989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683061f55f48cc917ee9747312cf74ee89f6dcb4576bc596a8c977b0eaf98e30`  
		Last Modified: Tue, 27 Oct 2020 18:41:56 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46428d67d6c50ed10e91275da1951cb79c531169d09a64c08b7626a3968469e8`  
		Last Modified: Tue, 27 Oct 2020 18:41:55 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.5.5` - linux; 386

```console
$ docker pull vault@sha256:de323dceeb2a37699470c8560310eebbde81e9f42a3d70fa9bd511f29ad5a2c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.9 MB (52948473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7df434d89d5b37542ec088003fb0bd2e1860472e29d1cf7eb5c685f4e06217c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Tue, 27 Oct 2020 18:58:40 GMT
ARG VAULT_VERSION=1.5.5
# Tue, 27 Oct 2020 18:58:41 GMT
# ARGS: VAULT_VERSION=1.5.5
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 27 Oct 2020 18:58:48 GMT
# ARGS: VAULT_VERSION=1.5.5
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 27 Oct 2020 18:58:49 GMT
# ARGS: VAULT_VERSION=1.5.5
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 27 Oct 2020 18:58:49 GMT
VOLUME [/vault/logs]
# Tue, 27 Oct 2020 18:58:49 GMT
VOLUME [/vault/file]
# Tue, 27 Oct 2020 18:58:49 GMT
EXPOSE 8200
# Tue, 27 Oct 2020 18:58:49 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 27 Oct 2020 18:58:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:58:50 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692404f5ab2258a860578dd4e1b2db60524b6141f41c75d08b0591d2077a6338`  
		Last Modified: Tue, 27 Oct 2020 18:59:01 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e294675be30c7d51d8d7e90fdc1df68c756499602a787f1ca9981ea65558c0c`  
		Last Modified: Tue, 27 Oct 2020 18:59:09 GMT  
		Size: 50.2 MB (50158105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35b6898967c5749dfc85958ae6c2d994b031ce445cc3a34d0e19f90b70a18ec`  
		Last Modified: Tue, 27 Oct 2020 18:59:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1962fb6943083f17d0d052a3c5e9de1d286ea9a52f18949c482b9b6cd87385c`  
		Last Modified: Tue, 27 Oct 2020 18:59:00 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.6.0`

```console
$ docker pull vault@sha256:175783dc9a177e103cf92d519ba53091c7c0c8fe29fe6555ecb678df9e3853ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.6.0` - linux; amd64

```console
$ docker pull vault@sha256:b04266db3e7ece92690df720fcf98ecf138a92ed3d1edc14dc86fe814c33ab9b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68720797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16f9627221417809465434ec0bfa6a7aa71e8c057ad742d6241635b174f16f00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Thu, 12 Nov 2020 01:37:53 GMT
ARG VAULT_VERSION=1.6.0
# Thu, 12 Nov 2020 01:37:54 GMT
# ARGS: VAULT_VERSION=1.6.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 12 Nov 2020 01:38:00 GMT
# ARGS: VAULT_VERSION=1.6.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 12 Nov 2020 01:38:01 GMT
# ARGS: VAULT_VERSION=1.6.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 12 Nov 2020 01:38:01 GMT
VOLUME [/vault/logs]
# Thu, 12 Nov 2020 01:38:02 GMT
VOLUME [/vault/file]
# Thu, 12 Nov 2020 01:38:02 GMT
EXPOSE 8200
# Thu, 12 Nov 2020 01:38:02 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 12 Nov 2020 01:38:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Nov 2020 01:38:02 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:551bb7f0c04c07a1bac7942ffff8330ca93c90233e2ba333694baf8936c99449`  
		Last Modified: Thu, 12 Nov 2020 01:38:18 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a083819c21ad0063c000a1029eba8d6a84460a185943aa670aef5e363472c51`  
		Last Modified: Thu, 12 Nov 2020 01:38:28 GMT  
		Size: 65.9 MB (65921973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47064f3768725dbadfb1de5717537bffbc3be3ccdc0dade491fdc258a2620192`  
		Last Modified: Thu, 12 Nov 2020 01:38:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1414769096159b9444c522870aa4418e67452f66bcaf10a59d356caf5e292f1f`  
		Last Modified: Thu, 12 Nov 2020 01:38:19 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.6.0` - linux; arm variant v6

```console
$ docker pull vault@sha256:f5e6af78549d376a2cb1ccedab8f16e0ce72ea40454ab45f488ce9bc280ecce2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.5 MB (63464369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ed2ef8b7af23b8b3e69583fa963ab1c2d8e64668e66ed0c98424ab3b8240a8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Thu, 12 Nov 2020 01:38:38 GMT
ARG VAULT_VERSION=1.6.0
# Thu, 12 Nov 2020 01:38:41 GMT
# ARGS: VAULT_VERSION=1.6.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 12 Nov 2020 01:38:54 GMT
# ARGS: VAULT_VERSION=1.6.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 12 Nov 2020 01:38:57 GMT
# ARGS: VAULT_VERSION=1.6.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 12 Nov 2020 01:38:58 GMT
VOLUME [/vault/logs]
# Thu, 12 Nov 2020 01:38:59 GMT
VOLUME [/vault/file]
# Thu, 12 Nov 2020 01:38:59 GMT
EXPOSE 8200
# Thu, 12 Nov 2020 01:39:00 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 12 Nov 2020 01:39:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Nov 2020 01:39:02 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbd9244c237bb7d62569dfe45af59fc9ee8999cbacefa7108557846913c19e6`  
		Last Modified: Thu, 12 Nov 2020 01:39:22 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db6c316f3ebbce8eec77650c2df98599323902d92284ac79dcad6670929581f`  
		Last Modified: Thu, 12 Nov 2020 01:39:40 GMT  
		Size: 60.9 MB (60888559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da34849c94cf96f49fd06750640e13c7ccc23a82977152341a76aedd97e635f3`  
		Last Modified: Thu, 12 Nov 2020 01:39:21 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7671ee5df4e85bd41d97074a98427aa71fb29931a6efcbc53dfdad2130dedd`  
		Last Modified: Thu, 12 Nov 2020 01:39:22 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.6.0` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:109ed1ae1ad667579a9206b45b71e1223482ebfa1ec3ba5ee8c0e971001eeb8e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.8 MB (64803536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae3c7801f9efac892d6ab87357a13290e8dc248b64dfd8402ac00cf288f76187`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Thu, 12 Nov 2020 01:50:53 GMT
ARG VAULT_VERSION=1.6.0
# Thu, 12 Nov 2020 01:50:55 GMT
# ARGS: VAULT_VERSION=1.6.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 12 Nov 2020 01:51:05 GMT
# ARGS: VAULT_VERSION=1.6.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 12 Nov 2020 01:51:09 GMT
# ARGS: VAULT_VERSION=1.6.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 12 Nov 2020 01:51:09 GMT
VOLUME [/vault/logs]
# Thu, 12 Nov 2020 01:51:10 GMT
VOLUME [/vault/file]
# Thu, 12 Nov 2020 01:51:11 GMT
EXPOSE 8200
# Thu, 12 Nov 2020 01:51:12 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 12 Nov 2020 01:51:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Nov 2020 01:51:14 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a82fe048c6ee7881c34575283b7f6ab4cdd22c5e3e8d5b93141204e227f4cb9`  
		Last Modified: Thu, 12 Nov 2020 01:51:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c203aec1ae9f50dc6bd91da4d7e7b7c94b406389b38a2926a7de2cb6c30bbb9e`  
		Last Modified: Thu, 12 Nov 2020 01:51:45 GMT  
		Size: 62.1 MB (62081500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908b3797024efa1beb7aa136ae1a24b68f3a95a7eb7c92e96bacb5e73bb2e6d7`  
		Last Modified: Thu, 12 Nov 2020 01:51:33 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244ccae43fad707a04e811b6d78ad5a74b692c1c2e45f33f7d17451262c52c51`  
		Last Modified: Thu, 12 Nov 2020 01:51:32 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.6.0` - linux; 386

```console
$ docker pull vault@sha256:824bb5040883039b2e90b2aa3afef9d059b391950e488216bb3c55cfe6b2ea28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.8 MB (66774356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a23fe610a36d3a2891c2af2031f9670791e50a7ed03d0c225a1beeddb4ebdd5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Thu, 12 Nov 2020 00:40:00 GMT
ARG VAULT_VERSION=1.6.0
# Thu, 12 Nov 2020 00:40:00 GMT
# ARGS: VAULT_VERSION=1.6.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 12 Nov 2020 00:40:09 GMT
# ARGS: VAULT_VERSION=1.6.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 12 Nov 2020 00:40:10 GMT
# ARGS: VAULT_VERSION=1.6.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 12 Nov 2020 00:40:10 GMT
VOLUME [/vault/logs]
# Thu, 12 Nov 2020 00:40:10 GMT
VOLUME [/vault/file]
# Thu, 12 Nov 2020 00:40:11 GMT
EXPOSE 8200
# Thu, 12 Nov 2020 00:40:11 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 12 Nov 2020 00:40:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Nov 2020 00:40:11 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aaf6459e02812154a86c3341fe75defa214d371074b792a506ac8d63220516d`  
		Last Modified: Thu, 12 Nov 2020 00:40:27 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7febaec9f79a10cd5303fc6a057e92b045678e4162f258d5251661393bffdee7`  
		Last Modified: Thu, 12 Nov 2020 00:40:39 GMT  
		Size: 64.0 MB (63983993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a2ee5cb020be73766dcafac0e4f7fadb0697ec880c84e7c5d9d55f76328a5d`  
		Last Modified: Thu, 12 Nov 2020 00:40:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ce03e47bbd8b8ccda6d5f1054a86e2cda92e28c529d0680386b3263a3f3d1c`  
		Last Modified: Thu, 12 Nov 2020 00:40:27 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:latest`

```console
$ docker pull vault@sha256:175783dc9a177e103cf92d519ba53091c7c0c8fe29fe6555ecb678df9e3853ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:b04266db3e7ece92690df720fcf98ecf138a92ed3d1edc14dc86fe814c33ab9b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68720797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16f9627221417809465434ec0bfa6a7aa71e8c057ad742d6241635b174f16f00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Thu, 12 Nov 2020 01:37:53 GMT
ARG VAULT_VERSION=1.6.0
# Thu, 12 Nov 2020 01:37:54 GMT
# ARGS: VAULT_VERSION=1.6.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 12 Nov 2020 01:38:00 GMT
# ARGS: VAULT_VERSION=1.6.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 12 Nov 2020 01:38:01 GMT
# ARGS: VAULT_VERSION=1.6.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 12 Nov 2020 01:38:01 GMT
VOLUME [/vault/logs]
# Thu, 12 Nov 2020 01:38:02 GMT
VOLUME [/vault/file]
# Thu, 12 Nov 2020 01:38:02 GMT
EXPOSE 8200
# Thu, 12 Nov 2020 01:38:02 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 12 Nov 2020 01:38:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Nov 2020 01:38:02 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:551bb7f0c04c07a1bac7942ffff8330ca93c90233e2ba333694baf8936c99449`  
		Last Modified: Thu, 12 Nov 2020 01:38:18 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a083819c21ad0063c000a1029eba8d6a84460a185943aa670aef5e363472c51`  
		Last Modified: Thu, 12 Nov 2020 01:38:28 GMT  
		Size: 65.9 MB (65921973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47064f3768725dbadfb1de5717537bffbc3be3ccdc0dade491fdc258a2620192`  
		Last Modified: Thu, 12 Nov 2020 01:38:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1414769096159b9444c522870aa4418e67452f66bcaf10a59d356caf5e292f1f`  
		Last Modified: Thu, 12 Nov 2020 01:38:19 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:f5e6af78549d376a2cb1ccedab8f16e0ce72ea40454ab45f488ce9bc280ecce2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.5 MB (63464369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ed2ef8b7af23b8b3e69583fa963ab1c2d8e64668e66ed0c98424ab3b8240a8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Thu, 12 Nov 2020 01:38:38 GMT
ARG VAULT_VERSION=1.6.0
# Thu, 12 Nov 2020 01:38:41 GMT
# ARGS: VAULT_VERSION=1.6.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 12 Nov 2020 01:38:54 GMT
# ARGS: VAULT_VERSION=1.6.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 12 Nov 2020 01:38:57 GMT
# ARGS: VAULT_VERSION=1.6.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 12 Nov 2020 01:38:58 GMT
VOLUME [/vault/logs]
# Thu, 12 Nov 2020 01:38:59 GMT
VOLUME [/vault/file]
# Thu, 12 Nov 2020 01:38:59 GMT
EXPOSE 8200
# Thu, 12 Nov 2020 01:39:00 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 12 Nov 2020 01:39:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Nov 2020 01:39:02 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbd9244c237bb7d62569dfe45af59fc9ee8999cbacefa7108557846913c19e6`  
		Last Modified: Thu, 12 Nov 2020 01:39:22 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db6c316f3ebbce8eec77650c2df98599323902d92284ac79dcad6670929581f`  
		Last Modified: Thu, 12 Nov 2020 01:39:40 GMT  
		Size: 60.9 MB (60888559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da34849c94cf96f49fd06750640e13c7ccc23a82977152341a76aedd97e635f3`  
		Last Modified: Thu, 12 Nov 2020 01:39:21 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7671ee5df4e85bd41d97074a98427aa71fb29931a6efcbc53dfdad2130dedd`  
		Last Modified: Thu, 12 Nov 2020 01:39:22 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:109ed1ae1ad667579a9206b45b71e1223482ebfa1ec3ba5ee8c0e971001eeb8e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.8 MB (64803536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae3c7801f9efac892d6ab87357a13290e8dc248b64dfd8402ac00cf288f76187`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Thu, 12 Nov 2020 01:50:53 GMT
ARG VAULT_VERSION=1.6.0
# Thu, 12 Nov 2020 01:50:55 GMT
# ARGS: VAULT_VERSION=1.6.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 12 Nov 2020 01:51:05 GMT
# ARGS: VAULT_VERSION=1.6.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 12 Nov 2020 01:51:09 GMT
# ARGS: VAULT_VERSION=1.6.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 12 Nov 2020 01:51:09 GMT
VOLUME [/vault/logs]
# Thu, 12 Nov 2020 01:51:10 GMT
VOLUME [/vault/file]
# Thu, 12 Nov 2020 01:51:11 GMT
EXPOSE 8200
# Thu, 12 Nov 2020 01:51:12 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 12 Nov 2020 01:51:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Nov 2020 01:51:14 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a82fe048c6ee7881c34575283b7f6ab4cdd22c5e3e8d5b93141204e227f4cb9`  
		Last Modified: Thu, 12 Nov 2020 01:51:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c203aec1ae9f50dc6bd91da4d7e7b7c94b406389b38a2926a7de2cb6c30bbb9e`  
		Last Modified: Thu, 12 Nov 2020 01:51:45 GMT  
		Size: 62.1 MB (62081500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908b3797024efa1beb7aa136ae1a24b68f3a95a7eb7c92e96bacb5e73bb2e6d7`  
		Last Modified: Thu, 12 Nov 2020 01:51:33 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244ccae43fad707a04e811b6d78ad5a74b692c1c2e45f33f7d17451262c52c51`  
		Last Modified: Thu, 12 Nov 2020 01:51:32 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:824bb5040883039b2e90b2aa3afef9d059b391950e488216bb3c55cfe6b2ea28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.8 MB (66774356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a23fe610a36d3a2891c2af2031f9670791e50a7ed03d0c225a1beeddb4ebdd5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Thu, 12 Nov 2020 00:40:00 GMT
ARG VAULT_VERSION=1.6.0
# Thu, 12 Nov 2020 00:40:00 GMT
# ARGS: VAULT_VERSION=1.6.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 12 Nov 2020 00:40:09 GMT
# ARGS: VAULT_VERSION=1.6.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 12 Nov 2020 00:40:10 GMT
# ARGS: VAULT_VERSION=1.6.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 12 Nov 2020 00:40:10 GMT
VOLUME [/vault/logs]
# Thu, 12 Nov 2020 00:40:10 GMT
VOLUME [/vault/file]
# Thu, 12 Nov 2020 00:40:11 GMT
EXPOSE 8200
# Thu, 12 Nov 2020 00:40:11 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 12 Nov 2020 00:40:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Nov 2020 00:40:11 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aaf6459e02812154a86c3341fe75defa214d371074b792a506ac8d63220516d`  
		Last Modified: Thu, 12 Nov 2020 00:40:27 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7febaec9f79a10cd5303fc6a057e92b045678e4162f258d5251661393bffdee7`  
		Last Modified: Thu, 12 Nov 2020 00:40:39 GMT  
		Size: 64.0 MB (63983993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a2ee5cb020be73766dcafac0e4f7fadb0697ec880c84e7c5d9d55f76328a5d`  
		Last Modified: Thu, 12 Nov 2020 00:40:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ce03e47bbd8b8ccda6d5f1054a86e2cda92e28c529d0680386b3263a3f3d1c`  
		Last Modified: Thu, 12 Nov 2020 00:40:27 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
