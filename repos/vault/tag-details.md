<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:1.4.7`](#vault147)
-	[`vault:1.5.7`](#vault157)
-	[`vault:1.6.2`](#vault162)
-	[`vault:latest`](#vaultlatest)

## `vault:1.4.7`

```console
$ docker pull vault@sha256:6ca102ebda0660114f3267fec8dace692d4b62fdb09a22a9364faa2f5cf392d7
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
$ docker pull vault@sha256:1d7cdd3157c0730e403268c42b1664c7a12a357fed370a76dc83162e1fb7cd69
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48719706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cf464349a93aca1192e4aa9a035dec84f5b917d73df3f0b972c8586b40a73a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:55 GMT
ADD file:9e81f449863b2d114afc239efa445f3bed6ff45b123ea3aad271a5631ac4fa13 in / 
# Wed, 24 Feb 2021 20:50:56 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:37:59 GMT
ARG VAULT_VERSION=1.4.7
# Wed, 24 Feb 2021 23:38:01 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 24 Feb 2021 23:38:12 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 24 Feb 2021 23:38:14 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 24 Feb 2021 23:38:14 GMT
VOLUME [/vault/logs]
# Wed, 24 Feb 2021 23:38:15 GMT
VOLUME [/vault/file]
# Wed, 24 Feb 2021 23:38:16 GMT
EXPOSE 8200
# Wed, 24 Feb 2021 23:38:16 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 24 Feb 2021 23:38:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 23:38:18 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:615b6501bf7ed56706d638bf075665f504b2fee0bdebf905dcb8610bc9271fa4`  
		Last Modified: Wed, 24 Feb 2021 20:51:33 GMT  
		Size: 2.6 MB (2574559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c493d5d6dd04e6c618a2a05545ed54f80425ee3ed724bd08f61f6a9a23760fed`  
		Last Modified: Wed, 24 Feb 2021 23:39:21 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847e00f8e155413726c1399b24fd39855b85c0e5c680cd9899bd4ac4e57b8f6e`  
		Last Modified: Wed, 24 Feb 2021 23:39:33 GMT  
		Size: 46.1 MB (46141854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89c1e265b041edc4d3e36f1b93cfb8e3670c1453d620ee57fb087b52d9d72ed`  
		Last Modified: Wed, 24 Feb 2021 23:39:21 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faeaa20bf0f90081dc23437718d36e14f3932144e6327241205c897074f3e0a3`  
		Last Modified: Wed, 24 Feb 2021 23:39:21 GMT  
		Size: 1.8 KB (1818 bytes)  
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
$ docker pull vault@sha256:4f76a0ad04b1f6b83f4186497bb42bb82bbb7e15750ad9b9742b14fe53247c1b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50214387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1358829bba57123e84293125eaf1a27d8396505222731aabcf3f372f72238cf0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 24 Feb 2021 20:38:57 GMT
ADD file:b5ef4a4abd9ccb894bdda7a5750878d13fbac4746c7b173c5dc88cf4846fc976 in / 
# Wed, 24 Feb 2021 20:38:57 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 02:21:49 GMT
ARG VAULT_VERSION=1.4.7
# Thu, 25 Feb 2021 02:21:49 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 25 Feb 2021 02:21:57 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 25 Feb 2021 02:21:57 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 25 Feb 2021 02:21:58 GMT
VOLUME [/vault/logs]
# Thu, 25 Feb 2021 02:21:58 GMT
VOLUME [/vault/file]
# Thu, 25 Feb 2021 02:21:58 GMT
EXPOSE 8200
# Thu, 25 Feb 2021 02:21:58 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 25 Feb 2021 02:21:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 02:21:59 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:9c18aa22aceabbea5b9c3d26c1e449591c02413fb34b574d9f73520f3fea602b`  
		Last Modified: Wed, 24 Feb 2021 20:39:36 GMT  
		Size: 2.8 MB (2788780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:220fe3fe2a248b7bbddef3b57a8333e8349c3a4f2b4b8088465570dd607e42b3`  
		Last Modified: Thu, 25 Feb 2021 02:22:47 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f33503eda2cab545d58e547471cc38acbbbfc1b0dcb109c15dc189bcc678121`  
		Last Modified: Thu, 25 Feb 2021 02:22:57 GMT  
		Size: 47.4 MB (47422372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51623e219e50b3126c59ef2ed6f621991b25c868e5a7e34453816463b5a09c14`  
		Last Modified: Thu, 25 Feb 2021 02:22:47 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6583fe4c5d9d6fb03f4bd839494880a2eba1d286db9234b05aa9972ae6186c8d`  
		Last Modified: Thu, 25 Feb 2021 02:22:47 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.5.7`

```console
$ docker pull vault@sha256:7c5847d26b2f7466c903ab20204d3c6d3f18dafe59343a0d2e9079006ab1b795
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.5.7` - linux; amd64

```console
$ docker pull vault@sha256:2443c3e17c02c60c079ac3ebc3f6fd3e36655c4f451de767682d3b8f692df4a4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55007919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de1fc61ed288138ab4d6cdd38aba02a084f8f0f63906eaad984d33c379ae535b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Sat, 30 Jan 2021 02:33:09 GMT
ARG VAULT_VERSION=1.5.7
# Sat, 30 Jan 2021 02:33:10 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 30 Jan 2021 02:33:16 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 30 Jan 2021 02:33:17 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 30 Jan 2021 02:33:17 GMT
VOLUME [/vault/logs]
# Sat, 30 Jan 2021 02:33:17 GMT
VOLUME [/vault/file]
# Sat, 30 Jan 2021 02:33:17 GMT
EXPOSE 8200
# Sat, 30 Jan 2021 02:33:18 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 30 Jan 2021 02:33:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Jan 2021 02:33:18 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b545bb4f2158f5ec574a73c3feac64e9fef25668d590d2562c572a32e646c4f6`  
		Last Modified: Sat, 30 Jan 2021 02:33:47 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4f9b2ce8e41013c0feda2a3df8622c94a11520435341814afae5291605c058`  
		Last Modified: Sat, 30 Jan 2021 02:33:55 GMT  
		Size: 52.2 MB (52209102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369f7fbbbf66762a8ae79d79294718da4042d65c8b622de4c960e7442286831d`  
		Last Modified: Sat, 30 Jan 2021 02:33:46 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52517a528f12aa188a8af9ac19020a6995b2dfce51a107294ae27d1515abcfa6`  
		Last Modified: Sat, 30 Jan 2021 02:33:46 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.5.7` - linux; arm variant v6

```console
$ docker pull vault@sha256:29e18e929a36011901973283bd4fb7c0723fa8605f3ce60c99f6089134821831
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51563428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ebecacf8c1f7878517a0bdfc9b313dd3efcd661daaedcf07817766e44f70b20`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:55 GMT
ADD file:9e81f449863b2d114afc239efa445f3bed6ff45b123ea3aad271a5631ac4fa13 in / 
# Wed, 24 Feb 2021 20:50:56 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:37:28 GMT
ARG VAULT_VERSION=1.5.7
# Wed, 24 Feb 2021 23:37:29 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 24 Feb 2021 23:37:39 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 24 Feb 2021 23:37:42 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 24 Feb 2021 23:37:43 GMT
VOLUME [/vault/logs]
# Wed, 24 Feb 2021 23:37:45 GMT
VOLUME [/vault/file]
# Wed, 24 Feb 2021 23:37:47 GMT
EXPOSE 8200
# Wed, 24 Feb 2021 23:37:48 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 24 Feb 2021 23:37:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 23:37:50 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:615b6501bf7ed56706d638bf075665f504b2fee0bdebf905dcb8610bc9271fa4`  
		Last Modified: Wed, 24 Feb 2021 20:51:33 GMT  
		Size: 2.6 MB (2574559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427a2d6e45231426c91f9a0a1944ac81ffce942376ba018cf400b75504c49268`  
		Last Modified: Wed, 24 Feb 2021 23:39:00 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045524ab01e984686b84e13032ffbe082a603d939306b8d85c959d0f51952e27`  
		Last Modified: Wed, 24 Feb 2021 23:39:14 GMT  
		Size: 49.0 MB (48985575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6aa1c5eae8a4aebc90bd1d179561f8b161f59f5c282b09c484816f4484fa381`  
		Last Modified: Wed, 24 Feb 2021 23:39:00 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78833d0facb3234c90ed9bfe36fd6249bfe5f6f4523b017380487df1a390c0b`  
		Last Modified: Wed, 24 Feb 2021 23:39:00 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.5.7` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:313c82c781eb0ec5ec62f91c87b90fe515dfa9ededcad83f8a14b72734134b84
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51915953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5df73794759924d3ac56435da6c9e24f3daeb93aaa8ef93e023545f765391d94`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Sat, 30 Jan 2021 01:42:41 GMT
ARG VAULT_VERSION=1.5.7
# Sat, 30 Jan 2021 01:42:43 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 30 Jan 2021 01:42:50 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 30 Jan 2021 01:42:53 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 30 Jan 2021 01:42:53 GMT
VOLUME [/vault/logs]
# Sat, 30 Jan 2021 01:42:54 GMT
VOLUME [/vault/file]
# Sat, 30 Jan 2021 01:42:55 GMT
EXPOSE 8200
# Sat, 30 Jan 2021 01:42:56 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 30 Jan 2021 01:42:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Jan 2021 01:42:57 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3927cff41b82e525bc651b6a4352e9c474e4ae1c666b2ea8cff978cd7c46685f`  
		Last Modified: Sat, 30 Jan 2021 01:43:39 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bef71627eb4b72dd2f56b221b73ef4b246b91d43ef067e8c0447ace0b52c353`  
		Last Modified: Sat, 30 Jan 2021 01:43:49 GMT  
		Size: 49.2 MB (49193920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8e6febcfa1d0afb24867c0fa45ab61c8f10353e26dc62f7163820913fc857c`  
		Last Modified: Sat, 30 Jan 2021 01:43:39 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b01d62f28be7714ead019beab7a82fdd956d026db1d15851c65e1a61a15b47`  
		Last Modified: Sat, 30 Jan 2021 01:43:39 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.5.7` - linux; 386

```console
$ docker pull vault@sha256:2b9a146cb3edf59443b07c9901092aa9447db762cc4c6812a05556f4aeb8df29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53087089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:160aa0d3093f1bb269b73de17a736230fe9098cb77e6ffabb723dd2b6bf8cbf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 24 Feb 2021 20:38:57 GMT
ADD file:b5ef4a4abd9ccb894bdda7a5750878d13fbac4746c7b173c5dc88cf4846fc976 in / 
# Wed, 24 Feb 2021 20:38:57 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 02:21:32 GMT
ARG VAULT_VERSION=1.5.7
# Thu, 25 Feb 2021 02:21:33 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 25 Feb 2021 02:21:40 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 25 Feb 2021 02:21:41 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 25 Feb 2021 02:21:41 GMT
VOLUME [/vault/logs]
# Thu, 25 Feb 2021 02:21:41 GMT
VOLUME [/vault/file]
# Thu, 25 Feb 2021 02:21:42 GMT
EXPOSE 8200
# Thu, 25 Feb 2021 02:21:42 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 25 Feb 2021 02:21:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 02:21:43 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:9c18aa22aceabbea5b9c3d26c1e449591c02413fb34b574d9f73520f3fea602b`  
		Last Modified: Wed, 24 Feb 2021 20:39:36 GMT  
		Size: 2.8 MB (2788780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9240bb1b514f2b7f3e3efc49b5909c685a3670458a07d24f90336a58d93d97f`  
		Last Modified: Thu, 25 Feb 2021 02:22:33 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b86a4dc009f1af52e9dab22d96058e7f8df3ecf156b045864a7794bc8054376`  
		Last Modified: Thu, 25 Feb 2021 02:22:43 GMT  
		Size: 50.3 MB (50295073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1554a93ff68d03e54b6f47b347e0ea67562086c6a3b7ae18e3a7fc97c13d263d`  
		Last Modified: Thu, 25 Feb 2021 02:22:36 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80edd1e6ad27f1537e6e11ec372b34df9ca92a80feddd2940f1242a17b27c250`  
		Last Modified: Thu, 25 Feb 2021 02:22:33 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.6.2`

```console
$ docker pull vault@sha256:9c557f35cb5ec21aebafa33ae8ad3d32e657b950ee10696f9c5d25cd3d4b8db7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.6.2` - linux; amd64

```console
$ docker pull vault@sha256:3891ca2e808582c37ff79c661ec9924ae062014de01c4c663a636967d994b646
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68949623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64665835d5865560b564d53790462b462c0f41ab46f3231cc096ecb12eca0d1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Sat, 30 Jan 2021 02:32:55 GMT
ARG VAULT_VERSION=1.6.2
# Sat, 30 Jan 2021 02:32:56 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 30 Jan 2021 02:33:03 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 30 Jan 2021 02:33:04 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 30 Jan 2021 02:33:04 GMT
VOLUME [/vault/logs]
# Sat, 30 Jan 2021 02:33:04 GMT
VOLUME [/vault/file]
# Sat, 30 Jan 2021 02:33:04 GMT
EXPOSE 8200
# Sat, 30 Jan 2021 02:33:05 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 30 Jan 2021 02:33:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Jan 2021 02:33:05 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67dfcdbc8a1ac2e6a91b72add2019a61090701d2296c9d93c692e0ea05bf8568`  
		Last Modified: Sat, 30 Jan 2021 02:33:32 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dd4c26996b1bc521b486b20aec46d22d991358ca6365ea5646610c2e603f9f`  
		Last Modified: Sat, 30 Jan 2021 02:33:42 GMT  
		Size: 66.2 MB (66150803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b63ae1409e87ff85da01bdfad67a4e84e906999d6b56b066329ea50b8ffe5db`  
		Last Modified: Sat, 30 Jan 2021 02:33:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028736f26ea0214c8751295ed6cf7206f9027bf91f593dda5f86b3af5836db61`  
		Last Modified: Sat, 30 Jan 2021 02:33:33 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.6.2` - linux; arm variant v6

```console
$ docker pull vault@sha256:365d4f2b2c9c071f5d281a140339088c0bcea0564721c2ce1d883e78212faeb8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63644476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9cb2a69288286a05d90da8f4bf96e5694a4daa9bfca7dde532b9645812dd4ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:55 GMT
ADD file:9e81f449863b2d114afc239efa445f3bed6ff45b123ea3aad271a5631ac4fa13 in / 
# Wed, 24 Feb 2021 20:50:56 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:36:56 GMT
ARG VAULT_VERSION=1.6.2
# Wed, 24 Feb 2021 23:36:59 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 24 Feb 2021 23:37:11 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 24 Feb 2021 23:37:14 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 24 Feb 2021 23:37:14 GMT
VOLUME [/vault/logs]
# Wed, 24 Feb 2021 23:37:15 GMT
VOLUME [/vault/file]
# Wed, 24 Feb 2021 23:37:16 GMT
EXPOSE 8200
# Wed, 24 Feb 2021 23:37:16 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 24 Feb 2021 23:37:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 23:37:18 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:615b6501bf7ed56706d638bf075665f504b2fee0bdebf905dcb8610bc9271fa4`  
		Last Modified: Wed, 24 Feb 2021 20:51:33 GMT  
		Size: 2.6 MB (2574559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a155eb2b4c3461bb9c2d4b3092615ea5cd7c79024ed3321f3bc085ab3faf4e`  
		Last Modified: Wed, 24 Feb 2021 23:38:37 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7401d26ee49a2312a785a1ae464b59b3dccd26cdfefab0df9a530b8d0c1d2c24`  
		Last Modified: Wed, 24 Feb 2021 23:38:52 GMT  
		Size: 61.1 MB (61066624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0787200f38137064dae13bdf155b2dc3f0930b091e259776046f5bcb69b707d0`  
		Last Modified: Wed, 24 Feb 2021 23:38:37 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4d90f641b5ac0a6a14b19d230c617828f817743d0208b17f57163dfdbc619a`  
		Last Modified: Wed, 24 Feb 2021 23:38:37 GMT  
		Size: 1.8 KB (1818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.6.2` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:5d19dda73172eaf68f3f97351b8997d63fb81853025a6ec24af4045a2918c58e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (65003474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8165c0e602824c7a50eb305e3b94f2cb291fff4955dae9c88ff320dd82046357`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Sat, 30 Jan 2021 01:42:17 GMT
ARG VAULT_VERSION=1.6.2
# Sat, 30 Jan 2021 01:42:19 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 30 Jan 2021 01:42:27 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 30 Jan 2021 01:42:29 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 30 Jan 2021 01:42:30 GMT
VOLUME [/vault/logs]
# Sat, 30 Jan 2021 01:42:31 GMT
VOLUME [/vault/file]
# Sat, 30 Jan 2021 01:42:31 GMT
EXPOSE 8200
# Sat, 30 Jan 2021 01:42:32 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 30 Jan 2021 01:42:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Jan 2021 01:42:33 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31023140a16d939fd3316e5c013e735f5b2199ff4fd68d2ee3a8046626cd8825`  
		Last Modified: Sat, 30 Jan 2021 01:43:19 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d95b0dcc3cd0d10ba19db1130df6fec8abe5abdeafbb6fb16e9e7634d3d1c08`  
		Last Modified: Sat, 30 Jan 2021 01:43:32 GMT  
		Size: 62.3 MB (62281439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f111f51485939ae0297844d458175b5cd697e43042a289cf0fc11874abca00`  
		Last Modified: Sat, 30 Jan 2021 01:43:19 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c78851589d6695666800a4c5e2b12ad7d454e5819058701d71b6ae957ec368`  
		Last Modified: Sat, 30 Jan 2021 01:43:19 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.6.2` - linux; 386

```console
$ docker pull vault@sha256:f65d8e13320cd4b57dad4f027b1ca7ad8189c7e5506361119b74e477ca789b92
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (66979396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdf41b24780052937fb07f3f159ad9e799c57f8ef2d2f89eabc9cc3e7f3c674c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 24 Feb 2021 20:38:57 GMT
ADD file:b5ef4a4abd9ccb894bdda7a5750878d13fbac4746c7b173c5dc88cf4846fc976 in / 
# Wed, 24 Feb 2021 20:38:57 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 02:21:16 GMT
ARG VAULT_VERSION=1.6.2
# Thu, 25 Feb 2021 02:21:17 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 25 Feb 2021 02:21:25 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 25 Feb 2021 02:21:26 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 25 Feb 2021 02:21:26 GMT
VOLUME [/vault/logs]
# Thu, 25 Feb 2021 02:21:26 GMT
VOLUME [/vault/file]
# Thu, 25 Feb 2021 02:21:26 GMT
EXPOSE 8200
# Thu, 25 Feb 2021 02:21:27 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 25 Feb 2021 02:21:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 02:21:27 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:9c18aa22aceabbea5b9c3d26c1e449591c02413fb34b574d9f73520f3fea602b`  
		Last Modified: Wed, 24 Feb 2021 20:39:36 GMT  
		Size: 2.8 MB (2788780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0fc52b079229357fc9195698dc4303c0e212ed15301e27bb83fd11eedbe9e2`  
		Last Modified: Thu, 25 Feb 2021 02:22:10 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e63ce9a15940c0601a22101e5fd26d317785bcedbfe3109bdc8239cdc1c3bd8`  
		Last Modified: Thu, 25 Feb 2021 02:22:22 GMT  
		Size: 64.2 MB (64187381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd573b73273525828bd1f2b8a0ee74247d3ff81a81e3e3ad7570cc66cd04373`  
		Last Modified: Thu, 25 Feb 2021 02:22:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208e73e1767b2f4838dc4384ab6af198011b113124018ef666946a3dc1b3475f`  
		Last Modified: Thu, 25 Feb 2021 02:22:10 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:latest`

```console
$ docker pull vault@sha256:9c557f35cb5ec21aebafa33ae8ad3d32e657b950ee10696f9c5d25cd3d4b8db7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:3891ca2e808582c37ff79c661ec9924ae062014de01c4c663a636967d994b646
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68949623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64665835d5865560b564d53790462b462c0f41ab46f3231cc096ecb12eca0d1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Sat, 30 Jan 2021 02:32:55 GMT
ARG VAULT_VERSION=1.6.2
# Sat, 30 Jan 2021 02:32:56 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 30 Jan 2021 02:33:03 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 30 Jan 2021 02:33:04 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 30 Jan 2021 02:33:04 GMT
VOLUME [/vault/logs]
# Sat, 30 Jan 2021 02:33:04 GMT
VOLUME [/vault/file]
# Sat, 30 Jan 2021 02:33:04 GMT
EXPOSE 8200
# Sat, 30 Jan 2021 02:33:05 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 30 Jan 2021 02:33:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Jan 2021 02:33:05 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67dfcdbc8a1ac2e6a91b72add2019a61090701d2296c9d93c692e0ea05bf8568`  
		Last Modified: Sat, 30 Jan 2021 02:33:32 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dd4c26996b1bc521b486b20aec46d22d991358ca6365ea5646610c2e603f9f`  
		Last Modified: Sat, 30 Jan 2021 02:33:42 GMT  
		Size: 66.2 MB (66150803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b63ae1409e87ff85da01bdfad67a4e84e906999d6b56b066329ea50b8ffe5db`  
		Last Modified: Sat, 30 Jan 2021 02:33:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028736f26ea0214c8751295ed6cf7206f9027bf91f593dda5f86b3af5836db61`  
		Last Modified: Sat, 30 Jan 2021 02:33:33 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:365d4f2b2c9c071f5d281a140339088c0bcea0564721c2ce1d883e78212faeb8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63644476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9cb2a69288286a05d90da8f4bf96e5694a4daa9bfca7dde532b9645812dd4ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:55 GMT
ADD file:9e81f449863b2d114afc239efa445f3bed6ff45b123ea3aad271a5631ac4fa13 in / 
# Wed, 24 Feb 2021 20:50:56 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:36:56 GMT
ARG VAULT_VERSION=1.6.2
# Wed, 24 Feb 2021 23:36:59 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 24 Feb 2021 23:37:11 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 24 Feb 2021 23:37:14 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 24 Feb 2021 23:37:14 GMT
VOLUME [/vault/logs]
# Wed, 24 Feb 2021 23:37:15 GMT
VOLUME [/vault/file]
# Wed, 24 Feb 2021 23:37:16 GMT
EXPOSE 8200
# Wed, 24 Feb 2021 23:37:16 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 24 Feb 2021 23:37:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 23:37:18 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:615b6501bf7ed56706d638bf075665f504b2fee0bdebf905dcb8610bc9271fa4`  
		Last Modified: Wed, 24 Feb 2021 20:51:33 GMT  
		Size: 2.6 MB (2574559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a155eb2b4c3461bb9c2d4b3092615ea5cd7c79024ed3321f3bc085ab3faf4e`  
		Last Modified: Wed, 24 Feb 2021 23:38:37 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7401d26ee49a2312a785a1ae464b59b3dccd26cdfefab0df9a530b8d0c1d2c24`  
		Last Modified: Wed, 24 Feb 2021 23:38:52 GMT  
		Size: 61.1 MB (61066624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0787200f38137064dae13bdf155b2dc3f0930b091e259776046f5bcb69b707d0`  
		Last Modified: Wed, 24 Feb 2021 23:38:37 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4d90f641b5ac0a6a14b19d230c617828f817743d0208b17f57163dfdbc619a`  
		Last Modified: Wed, 24 Feb 2021 23:38:37 GMT  
		Size: 1.8 KB (1818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:5d19dda73172eaf68f3f97351b8997d63fb81853025a6ec24af4045a2918c58e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (65003474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8165c0e602824c7a50eb305e3b94f2cb291fff4955dae9c88ff320dd82046357`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Sat, 30 Jan 2021 01:42:17 GMT
ARG VAULT_VERSION=1.6.2
# Sat, 30 Jan 2021 01:42:19 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 30 Jan 2021 01:42:27 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 30 Jan 2021 01:42:29 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 30 Jan 2021 01:42:30 GMT
VOLUME [/vault/logs]
# Sat, 30 Jan 2021 01:42:31 GMT
VOLUME [/vault/file]
# Sat, 30 Jan 2021 01:42:31 GMT
EXPOSE 8200
# Sat, 30 Jan 2021 01:42:32 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 30 Jan 2021 01:42:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Jan 2021 01:42:33 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31023140a16d939fd3316e5c013e735f5b2199ff4fd68d2ee3a8046626cd8825`  
		Last Modified: Sat, 30 Jan 2021 01:43:19 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d95b0dcc3cd0d10ba19db1130df6fec8abe5abdeafbb6fb16e9e7634d3d1c08`  
		Last Modified: Sat, 30 Jan 2021 01:43:32 GMT  
		Size: 62.3 MB (62281439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f111f51485939ae0297844d458175b5cd697e43042a289cf0fc11874abca00`  
		Last Modified: Sat, 30 Jan 2021 01:43:19 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c78851589d6695666800a4c5e2b12ad7d454e5819058701d71b6ae957ec368`  
		Last Modified: Sat, 30 Jan 2021 01:43:19 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:f65d8e13320cd4b57dad4f027b1ca7ad8189c7e5506361119b74e477ca789b92
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (66979396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdf41b24780052937fb07f3f159ad9e799c57f8ef2d2f89eabc9cc3e7f3c674c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 24 Feb 2021 20:38:57 GMT
ADD file:b5ef4a4abd9ccb894bdda7a5750878d13fbac4746c7b173c5dc88cf4846fc976 in / 
# Wed, 24 Feb 2021 20:38:57 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 02:21:16 GMT
ARG VAULT_VERSION=1.6.2
# Thu, 25 Feb 2021 02:21:17 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 25 Feb 2021 02:21:25 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 25 Feb 2021 02:21:26 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 25 Feb 2021 02:21:26 GMT
VOLUME [/vault/logs]
# Thu, 25 Feb 2021 02:21:26 GMT
VOLUME [/vault/file]
# Thu, 25 Feb 2021 02:21:26 GMT
EXPOSE 8200
# Thu, 25 Feb 2021 02:21:27 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 25 Feb 2021 02:21:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 02:21:27 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:9c18aa22aceabbea5b9c3d26c1e449591c02413fb34b574d9f73520f3fea602b`  
		Last Modified: Wed, 24 Feb 2021 20:39:36 GMT  
		Size: 2.8 MB (2788780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0fc52b079229357fc9195698dc4303c0e212ed15301e27bb83fd11eedbe9e2`  
		Last Modified: Thu, 25 Feb 2021 02:22:10 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e63ce9a15940c0601a22101e5fd26d317785bcedbfe3109bdc8239cdc1c3bd8`  
		Last Modified: Thu, 25 Feb 2021 02:22:22 GMT  
		Size: 64.2 MB (64187381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd573b73273525828bd1f2b8a0ee74247d3ff81a81e3e3ad7570cc66cd04373`  
		Last Modified: Thu, 25 Feb 2021 02:22:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208e73e1767b2f4838dc4384ab6af198011b113124018ef666946a3dc1b3475f`  
		Last Modified: Thu, 25 Feb 2021 02:22:10 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
