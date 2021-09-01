<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:1.5.9`](#vault159)
-	[`vault:1.6.6`](#vault166)
-	[`vault:1.7.4`](#vault174)
-	[`vault:1.8.2`](#vault182)
-	[`vault:latest`](#vaultlatest)

## `vault:1.5.9`

```console
$ docker pull vault@sha256:d5e1ba7d9ab13cd681b11aa0b6ad6c44edd95f11c1169287b7b46a3750c599d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.5.9` - linux; amd64

```console
$ docker pull vault@sha256:173212142be586a2558b2ff8cf701632c49dcd46cd522c69ff55265258d5bb74
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.1 MB (55101261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9be2afbafea177c86d7b64ed1ff6882843a7e3d4c6630ee73fcf0af5d066f960`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 06:17:28 GMT
ARG VAULT_VERSION=1.5.9
# Wed, 01 Sep 2021 06:17:29 GMT
# ARGS: VAULT_VERSION=1.5.9
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 01 Sep 2021 06:17:38 GMT
# ARGS: VAULT_VERSION=1.5.9
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 01 Sep 2021 06:17:39 GMT
# ARGS: VAULT_VERSION=1.5.9
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 01 Sep 2021 06:17:39 GMT
VOLUME [/vault/logs]
# Wed, 01 Sep 2021 06:17:39 GMT
VOLUME [/vault/file]
# Wed, 01 Sep 2021 06:17:39 GMT
EXPOSE 8200
# Wed, 01 Sep 2021 06:17:40 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 01 Sep 2021 06:17:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 06:17:40 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6aff56fc2a66d6bdeb572825b481b1f259938d30c7986413d03f8ac63de529e`  
		Last Modified: Wed, 01 Sep 2021 06:17:56 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f81065ca5f94fdf96731590daeaf8625fe6d2ea5400126d45786af2ddc2389d`  
		Last Modified: Wed, 01 Sep 2021 06:18:04 GMT  
		Size: 52.3 MB (52283917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ec1ddb9f38f190ec9c39107d0be9b4c858b4393f22a66ddba652cb4acb6088`  
		Last Modified: Wed, 01 Sep 2021 06:17:57 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9dcfeccf207be3e2d11842039700746f151e2b4ad65f253f23141b4517e4e6`  
		Last Modified: Wed, 01 Sep 2021 06:17:56 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.5.9` - linux; arm variant v6

```console
$ docker pull vault@sha256:e2d2a36481434e70b156344f0f909fbf8c22f8d3b1f252304502453228df8068
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51676395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f624a50fd6e60f468a38f2773f681618d2ac97757084862dfc7ea5bba7bc75f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 30 Jul 2021 17:49:55 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Fri, 30 Jul 2021 17:49:55 GMT
CMD ["/bin/sh"]
# Sat, 31 Jul 2021 07:22:46 GMT
ARG VAULT_VERSION=1.5.9
# Sat, 31 Jul 2021 07:22:47 GMT
# ARGS: VAULT_VERSION=1.5.9
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 31 Jul 2021 07:23:00 GMT
# ARGS: VAULT_VERSION=1.5.9
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 31 Jul 2021 07:23:02 GMT
# ARGS: VAULT_VERSION=1.5.9
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 31 Jul 2021 07:23:03 GMT
VOLUME [/vault/logs]
# Sat, 31 Jul 2021 07:23:03 GMT
VOLUME [/vault/file]
# Sat, 31 Jul 2021 07:23:04 GMT
EXPOSE 8200
# Sat, 31 Jul 2021 07:23:04 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 31 Jul 2021 07:23:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 31 Jul 2021 07:23:05 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc1b7a148db6c583a6a27f5e8613ae1b1c014e20d85fd56a77b2066dccc073d`  
		Last Modified: Sat, 31 Jul 2021 07:25:52 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0be7574872e5527c384b760db812d8e322b94483968883a679a28bdd0c921cc`  
		Last Modified: Sat, 31 Jul 2021 07:26:08 GMT  
		Size: 49.1 MB (49050993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e366ed5ca33bd6e24e5bbbf3ce0393eec99a738b2edd755792a43519c498f4`  
		Last Modified: Sat, 31 Jul 2021 07:25:52 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d42568f4ae17b196a10e05089de9e618fe6f8bc0078ac4b48d921cd8648593d`  
		Last Modified: Sat, 31 Jul 2021 07:25:52 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.5.9` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:a0e2b30562b8f154d20aa3572bb605895f2b60a2f38efb6f753e79bb29e1602e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.0 MB (51980486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:338eab721d389b8ad81936559c48b6c8db8890320c6cc17006f3c95bfe221c75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:15:51 GMT
ARG VAULT_VERSION=1.5.9
# Wed, 16 Jun 2021 11:15:51 GMT
# ARGS: VAULT_VERSION=1.5.9
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 16 Jun 2021 11:15:57 GMT
# ARGS: VAULT_VERSION=1.5.9
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 16 Jun 2021 11:15:58 GMT
# ARGS: VAULT_VERSION=1.5.9
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 16 Jun 2021 11:15:58 GMT
VOLUME [/vault/logs]
# Wed, 16 Jun 2021 11:15:58 GMT
VOLUME [/vault/file]
# Wed, 16 Jun 2021 11:15:58 GMT
EXPOSE 8200
# Wed, 16 Jun 2021 11:15:59 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 16 Jun 2021 11:15:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:15:59 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044ee0e2273e5939b76be629e500ad1691f5c16089f9d82b31b843d8924614cd`  
		Last Modified: Wed, 16 Jun 2021 11:16:57 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833a61638dbcd3e8b3d6d0e48bb117607c84f5471c9dabb4dc3d10489efc0f13`  
		Last Modified: Wed, 16 Jun 2021 11:17:05 GMT  
		Size: 49.3 MB (49265191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c2ef244dc2507fb8370c79b513bcd648b7f6b77f576e03abb67b52abe5e88a9`  
		Last Modified: Wed, 16 Jun 2021 11:16:57 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba72ece798b86a75c30c528474eed98b236bfe0c2fb6fbb835e19040af70e69`  
		Last Modified: Wed, 16 Jun 2021 11:16:57 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.5.9` - linux; 386

```console
$ docker pull vault@sha256:8eda22213ebaa53d0da65d60aa5d165fb15d5ef50d0b75b7746c83751bd6a062
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53174898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56ed990de33c2864ce228635346696542eb4a96fedc8c641fde94dcd874495cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 31 Aug 2021 21:23:28 GMT
ADD file:fb9d541cffc3a5660d23426ba847aa696b59a9d7f14e00ba0a63b28c9ec272c0 in / 
# Tue, 31 Aug 2021 21:23:29 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 03:08:38 GMT
ARG VAULT_VERSION=1.5.9
# Wed, 01 Sep 2021 03:08:39 GMT
# ARGS: VAULT_VERSION=1.5.9
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 01 Sep 2021 03:08:49 GMT
# ARGS: VAULT_VERSION=1.5.9
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 01 Sep 2021 03:08:51 GMT
# ARGS: VAULT_VERSION=1.5.9
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 01 Sep 2021 03:08:51 GMT
VOLUME [/vault/logs]
# Wed, 01 Sep 2021 03:08:51 GMT
VOLUME [/vault/file]
# Wed, 01 Sep 2021 03:08:52 GMT
EXPOSE 8200
# Wed, 01 Sep 2021 03:08:52 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 01 Sep 2021 03:08:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 03:08:52 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:4ed7d06bd90bc8d13b87220ccc6204a7d235ec943be9fb4289d856f9ff0a5b7b`  
		Last Modified: Tue, 31 Aug 2021 21:24:28 GMT  
		Size: 2.8 MB (2821095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523ce25561ac0325674e64884dc7c4eb1cb6c4aa1147eee148249b2983cc1718`  
		Last Modified: Wed, 01 Sep 2021 03:09:16 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585e9123868f1da6989289e30eeac6d3d3aae86e5bec1a20b184128ba2d3d206`  
		Last Modified: Wed, 01 Sep 2021 03:09:24 GMT  
		Size: 50.4 MB (50350539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd4b9ddbe59055723675960178d1e9604bf23b4079b9d11caa540fe35663293`  
		Last Modified: Wed, 01 Sep 2021 03:09:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:682e0037c325651603faa67fa8ff2cb19b175402882ebd9747a5bbf95954085f`  
		Last Modified: Wed, 01 Sep 2021 03:09:16 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.6.6`

```console
$ docker pull vault@sha256:c1c52004538ff11dfc51868c4aa74f34d1bba7ca756b6b2bd9232ea1b4a7ebc0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.6.6` - linux; amd64

```console
$ docker pull vault@sha256:2ab4a840f90828511f987b0686dc86120bd4a53a80f555478d73f3aaac3d04bc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69083601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7189bafda5c0948e6b867d775d4382b1d36dd71d66d3b9fbe1e744bf12b814a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 17:50:08 GMT
ARG VAULT_VERSION=1.6.6
# Fri, 27 Aug 2021 17:50:09 GMT
# ARGS: VAULT_VERSION=1.6.6
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 27 Aug 2021 17:50:16 GMT
# ARGS: VAULT_VERSION=1.6.6
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 27 Aug 2021 17:50:17 GMT
# ARGS: VAULT_VERSION=1.6.6
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 27 Aug 2021 17:50:18 GMT
VOLUME [/vault/logs]
# Fri, 27 Aug 2021 17:50:18 GMT
VOLUME [/vault/file]
# Fri, 27 Aug 2021 17:50:18 GMT
EXPOSE 8200
# Fri, 27 Aug 2021 17:50:18 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 Aug 2021 17:50:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 17:50:19 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aac3f61bf08971372d3e11896173f7c6a6667ce79da1e5e2f3aa03835f4167b`  
		Last Modified: Fri, 27 Aug 2021 17:51:11 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141b88d1f0da6830c3d8ecfaec11c5a536467c8e7d36eecf11c89d2040ec4999`  
		Last Modified: Fri, 27 Aug 2021 17:51:22 GMT  
		Size: 66.3 MB (66265879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d104c1e3b0838379e6cc6a7a00968d0177814e4d074e9ae7dae4a506cc67aa5e`  
		Last Modified: Fri, 27 Aug 2021 17:51:11 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ec9f7ff036aa23a22a3a8a3501a347ba23ac9d6b7712ff63f0b2afdce7b0ae`  
		Last Modified: Fri, 27 Aug 2021 17:51:11 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.6.6` - linux; arm variant v6

```console
$ docker pull vault@sha256:b043e9759f11a68fc190b74a3c0da4d869e105c63ce2ba08e86b68ffe2c4d5f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63815133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:180eb8c950c9bd167322fb52e568dfd3fc45b49664e2d4b6beb7093bf3bec26e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 18:18:04 GMT
ARG VAULT_VERSION=1.6.6
# Fri, 27 Aug 2021 18:18:06 GMT
# ARGS: VAULT_VERSION=1.6.6
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 27 Aug 2021 18:18:25 GMT
# ARGS: VAULT_VERSION=1.6.6
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 27 Aug 2021 18:18:27 GMT
# ARGS: VAULT_VERSION=1.6.6
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 27 Aug 2021 18:18:27 GMT
VOLUME [/vault/logs]
# Fri, 27 Aug 2021 18:18:28 GMT
VOLUME [/vault/file]
# Fri, 27 Aug 2021 18:18:28 GMT
EXPOSE 8200
# Fri, 27 Aug 2021 18:18:29 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 Aug 2021 18:18:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 18:18:29 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29351c1bbaa08344691dac7a3236cb7703d660282d4e4c31f7b487c6720de177`  
		Last Modified: Fri, 27 Aug 2021 18:20:40 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7eab72ffd4e69d740fa12d8438813381ea4a5cb0cbe90c64be41310598429f`  
		Last Modified: Fri, 27 Aug 2021 18:21:13 GMT  
		Size: 61.2 MB (61184408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17be93b849be315aa5daa6794c464dd38bdc1855e5d9b18abe1e32dddfa21cb`  
		Last Modified: Fri, 27 Aug 2021 18:20:40 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6417a3f94ce8cc58c5ddada1a6969f225080f825842e03f270a41d6e593a3bd6`  
		Last Modified: Fri, 27 Aug 2021 18:20:40 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.6.6` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:ebe6730f7387b0cf7dd86d82a7cb266809581c0571b6f9984b2d3a8680900872
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.1 MB (65107200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b893538f117fa17ace7b170b249ded9c9ecc051060e05d2a7d0cdeeeeed718f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 18:11:27 GMT
ARG VAULT_VERSION=1.6.6
# Fri, 27 Aug 2021 18:11:27 GMT
# ARGS: VAULT_VERSION=1.6.6
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 27 Aug 2021 18:11:34 GMT
# ARGS: VAULT_VERSION=1.6.6
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 27 Aug 2021 18:11:35 GMT
# ARGS: VAULT_VERSION=1.6.6
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 27 Aug 2021 18:11:35 GMT
VOLUME [/vault/logs]
# Fri, 27 Aug 2021 18:11:35 GMT
VOLUME [/vault/file]
# Fri, 27 Aug 2021 18:11:35 GMT
EXPOSE 8200
# Fri, 27 Aug 2021 18:11:35 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 Aug 2021 18:11:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 18:11:36 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e13542354f95c1040749fa96e377b59b38b19240ec6b02326c402f3376ca0e`  
		Last Modified: Fri, 27 Aug 2021 18:12:37 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e9694ea77372c1c4afbda736f4a0946162d62c04091137f7d00a38545e4a36`  
		Last Modified: Fri, 27 Aug 2021 18:12:46 GMT  
		Size: 62.4 MB (62392097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c644733f96dd2a9b3ab37eb0da2506c5f710d0821f3861ffcf70f614670bffc`  
		Last Modified: Fri, 27 Aug 2021 18:12:36 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7900e7bd43151ae79874464e82d3d3a289c5071cee394e005a226715d180307`  
		Last Modified: Fri, 27 Aug 2021 18:12:37 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.6.6` - linux; 386

```console
$ docker pull vault@sha256:ab6c39fe0a662c97e16aab234c8053c5cd6072915440a5a83f76ba3dd5baa724
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67129797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a95b10091a14e547ebd979356b7b998b6612cfc89ef9ffb7210eb95c53dc3760`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 17:51:19 GMT
ARG VAULT_VERSION=1.6.6
# Fri, 27 Aug 2021 17:51:20 GMT
# ARGS: VAULT_VERSION=1.6.6
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 27 Aug 2021 17:51:29 GMT
# ARGS: VAULT_VERSION=1.6.6
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 27 Aug 2021 17:51:30 GMT
# ARGS: VAULT_VERSION=1.6.6
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 27 Aug 2021 17:51:30 GMT
VOLUME [/vault/logs]
# Fri, 27 Aug 2021 17:51:30 GMT
VOLUME [/vault/file]
# Fri, 27 Aug 2021 17:51:30 GMT
EXPOSE 8200
# Fri, 27 Aug 2021 17:51:31 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 Aug 2021 17:51:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 17:51:31 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6819f90b8c073f1a9125fcc5f2ae191d7f6770812c54e1b6128100e788860a38`  
		Last Modified: Fri, 27 Aug 2021 17:52:35 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2165926ee2a5924d6c40e2a274619f9340dcf2724d0739e33dd6d19fb91c524b`  
		Last Modified: Fri, 27 Aug 2021 17:52:45 GMT  
		Size: 64.3 MB (64303663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead213d3b1544ddca27117b72041ac8a8301ee283e46472dc4d7e264ee81a5b9`  
		Last Modified: Fri, 27 Aug 2021 17:52:35 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb5c5de64052b0960fa9e87d42acd5db847be63af61f3c2e645319d965600dc`  
		Last Modified: Fri, 27 Aug 2021 17:52:35 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.7.4`

```console
$ docker pull vault@sha256:33fba890b7dc7e9f9cc93a291c3eb6708ef5f7f0c864634e32380f8792d08847
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.7.4` - linux; amd64

```console
$ docker pull vault@sha256:2f866f4e188c5818020bf7f105335f1742dfe740fc901808569da4c7ca5e8f3e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73973919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8018c2cd6b9f77a2ef54b13f1bf91dcefa24e316af1f77d0214979fc6ca6e1ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 17:49:50 GMT
ARG VAULT_VERSION=1.7.4
# Fri, 27 Aug 2021 17:49:51 GMT
# ARGS: VAULT_VERSION=1.7.4
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 27 Aug 2021 17:50:02 GMT
# ARGS: VAULT_VERSION=1.7.4
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 27 Aug 2021 17:50:04 GMT
# ARGS: VAULT_VERSION=1.7.4
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 27 Aug 2021 17:50:04 GMT
VOLUME [/vault/logs]
# Fri, 27 Aug 2021 17:50:04 GMT
VOLUME [/vault/file]
# Fri, 27 Aug 2021 17:50:04 GMT
EXPOSE 8200
# Fri, 27 Aug 2021 17:50:05 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 Aug 2021 17:50:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 17:50:05 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199d1cb0ef281e2836d189de9e20ff473c996b942fd49d983a6820d36b92cabc`  
		Last Modified: Fri, 27 Aug 2021 17:50:54 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6873107b6689978c6bcfc4961d59fd3e2bda40ea310f01d6b697527fa9d9779`  
		Last Modified: Fri, 27 Aug 2021 17:51:03 GMT  
		Size: 71.2 MB (71156198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccaa5df58c546923b6efcf03ddc42c61793fcbd921026ee89b59e1a591ac3f23`  
		Last Modified: Fri, 27 Aug 2021 17:50:54 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cfbc5390692721a41d5f0e93d85d92d8c4258e8a24dc3436b3a17d9fddb9863`  
		Last Modified: Fri, 27 Aug 2021 17:50:54 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.7.4` - linux; arm variant v6

```console
$ docker pull vault@sha256:ce2634555f6fd630a4d8839e2eaa5c0b5694601d8117e6ba480f10b7a2e9201a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67809545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60d04f2098f5b14bafe3b9f0b99f9b10dd3c993e87134c26ec72bb6f5769e7f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 18:17:22 GMT
ARG VAULT_VERSION=1.7.4
# Fri, 27 Aug 2021 18:17:24 GMT
# ARGS: VAULT_VERSION=1.7.4
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 27 Aug 2021 18:17:46 GMT
# ARGS: VAULT_VERSION=1.7.4
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 27 Aug 2021 18:17:48 GMT
# ARGS: VAULT_VERSION=1.7.4
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 27 Aug 2021 18:17:49 GMT
VOLUME [/vault/logs]
# Fri, 27 Aug 2021 18:17:49 GMT
VOLUME [/vault/file]
# Fri, 27 Aug 2021 18:17:50 GMT
EXPOSE 8200
# Fri, 27 Aug 2021 18:17:50 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 Aug 2021 18:17:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 18:17:51 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d39720118de50e5fd87ad2faac2c5602415247aa76255ca5155d23ec19234e`  
		Last Modified: Fri, 27 Aug 2021 18:19:57 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8239227a3890fc8b9b3497044fc586126a9ebb3f08045bb4f786775c9f270adb`  
		Last Modified: Fri, 27 Aug 2021 18:20:32 GMT  
		Size: 65.2 MB (65178822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db4eefef083c09378238168f459092bb072eb7217f2250f99602c25900db071`  
		Last Modified: Fri, 27 Aug 2021 18:19:56 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fc2368466782baa1c7ba3fe0ba119d0c5d1d1eda4548490c0ca619997b53aa`  
		Last Modified: Fri, 27 Aug 2021 18:19:56 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.7.4` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:aa2df32eb5458d2edd6d8a22fe2b23d97bf41d54f47aec0e5d0a234ab608bf99
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69747903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea4c87cd5c4a221635bcf414376f7841ec54994b2d659550da70e266183ae867`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 18:11:07 GMT
ARG VAULT_VERSION=1.7.4
# Fri, 27 Aug 2021 18:11:08 GMT
# ARGS: VAULT_VERSION=1.7.4
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 27 Aug 2021 18:11:19 GMT
# ARGS: VAULT_VERSION=1.7.4
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 27 Aug 2021 18:11:20 GMT
# ARGS: VAULT_VERSION=1.7.4
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 27 Aug 2021 18:11:20 GMT
VOLUME [/vault/logs]
# Fri, 27 Aug 2021 18:11:20 GMT
VOLUME [/vault/file]
# Fri, 27 Aug 2021 18:11:21 GMT
EXPOSE 8200
# Fri, 27 Aug 2021 18:11:21 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 Aug 2021 18:11:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 18:11:21 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9a6f3c97a35b54c8976a5b44cbfef31fd77f4e529fbbf4ba245e5136885510`  
		Last Modified: Fri, 27 Aug 2021 18:12:19 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da780d16cb9c9ac59d52fd2c4c5f9e815885a0ed4e70b5a7bbfbb3bbdbd00a08`  
		Last Modified: Fri, 27 Aug 2021 18:12:28 GMT  
		Size: 67.0 MB (67032799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f002bdb046b3c0aa35929ac0c895dcc569ffc80ec45c4d9019457f173bb36db6`  
		Last Modified: Fri, 27 Aug 2021 18:12:18 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71b1b0420bd6c73dbebd90f298653e2aeb6064ae3664ba91243dbf12551c1f6`  
		Last Modified: Fri, 27 Aug 2021 18:12:18 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.7.4` - linux; 386

```console
$ docker pull vault@sha256:db88d6ebcd7a587fa17dfed73a756de2a7b9a4ec21bf019e6c03a11f8688f1bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.8 MB (71825731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:644ef1abf63d0a97872a69c6579803edb63daebad2c47f88e660981315e44d6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 17:51:00 GMT
ARG VAULT_VERSION=1.7.4
# Fri, 27 Aug 2021 17:51:01 GMT
# ARGS: VAULT_VERSION=1.7.4
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 27 Aug 2021 17:51:12 GMT
# ARGS: VAULT_VERSION=1.7.4
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 27 Aug 2021 17:51:13 GMT
# ARGS: VAULT_VERSION=1.7.4
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 27 Aug 2021 17:51:13 GMT
VOLUME [/vault/logs]
# Fri, 27 Aug 2021 17:51:14 GMT
VOLUME [/vault/file]
# Fri, 27 Aug 2021 17:51:14 GMT
EXPOSE 8200
# Fri, 27 Aug 2021 17:51:14 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 Aug 2021 17:51:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 17:51:15 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77cd6a7c03983200092505a74e05d27bce43325711882d10333becd2fd0f521`  
		Last Modified: Fri, 27 Aug 2021 17:52:16 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53201d9f3b6f92abf916e016678f815a45610ee55f057d97f0e4b46f606695a3`  
		Last Modified: Fri, 27 Aug 2021 17:52:27 GMT  
		Size: 69.0 MB (68999599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c85d5e3bf0b34627ac0eb910062c51b70d38a73a4b0a2b3f9d61015c34697b`  
		Last Modified: Fri, 27 Aug 2021 17:52:16 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3551b055dc37f2c970837de5b70a45c673b7edee3b893463626bb78d4bb2b2`  
		Last Modified: Fri, 27 Aug 2021 17:52:16 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.8.2`

```console
$ docker pull vault@sha256:1422cccf59c78e046576e84612202334d1f7d995091d33f0e00141c3b075d0db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.8.2` - linux; amd64

```console
$ docker pull vault@sha256:79c1850dfcd98a496792e87908ce5d56f9293e27fb2d0b734aede341dadd69aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.5 MB (70451820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b8a82753be914c1950b74360978eeb2c68de8550b9696f19903c9fad2a1b48c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 17:49:29 GMT
ARG VAULT_VERSION=1.8.2
# Fri, 27 Aug 2021 17:49:29 GMT
# ARGS: VAULT_VERSION=1.8.2
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 27 Aug 2021 17:49:44 GMT
# ARGS: VAULT_VERSION=1.8.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 27 Aug 2021 17:49:45 GMT
# ARGS: VAULT_VERSION=1.8.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 27 Aug 2021 17:49:45 GMT
VOLUME [/vault/logs]
# Fri, 27 Aug 2021 17:49:45 GMT
VOLUME [/vault/file]
# Fri, 27 Aug 2021 17:49:45 GMT
EXPOSE 8200
# Fri, 27 Aug 2021 17:49:46 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 Aug 2021 17:49:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 17:49:46 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985e31a6bb65ae8ae336ae741cb08cb354fc42dc6685f50b679aff4364fb8311`  
		Last Modified: Fri, 27 Aug 2021 17:50:33 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0458da6383c22ad93107f4eab8b19313efe64eae1c4aaa61d6f74ca6a14cdd5d`  
		Last Modified: Fri, 27 Aug 2021 17:50:43 GMT  
		Size: 67.6 MB (67634098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be96eae97a36426ae377bea74c0bb67bcff4559776ddb2adadb14ee92504c48`  
		Last Modified: Fri, 27 Aug 2021 17:50:33 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db08138f178f2d0dd4005b7e4550d8f43d9b99c382b91e4a2d077befd6f8f01`  
		Last Modified: Fri, 27 Aug 2021 17:50:33 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.8.2` - linux; arm variant v6

```console
$ docker pull vault@sha256:6aebcc5b1f9eedbe7e5e72589cc09f06489cf0d8d01e9014ac01b98c0f11e7e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.8 MB (64843871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49c7f65637cae381ef8e4a74113373911a7f37433ea424c4c5c7dd87222a1ae6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 18:16:43 GMT
ARG VAULT_VERSION=1.8.2
# Fri, 27 Aug 2021 18:16:45 GMT
# ARGS: VAULT_VERSION=1.8.2
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 27 Aug 2021 18:17:06 GMT
# ARGS: VAULT_VERSION=1.8.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 27 Aug 2021 18:17:08 GMT
# ARGS: VAULT_VERSION=1.8.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 27 Aug 2021 18:17:09 GMT
VOLUME [/vault/logs]
# Fri, 27 Aug 2021 18:17:09 GMT
VOLUME [/vault/file]
# Fri, 27 Aug 2021 18:17:10 GMT
EXPOSE 8200
# Fri, 27 Aug 2021 18:17:10 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 Aug 2021 18:17:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 18:17:11 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcff2c885efceb6b909c389313f1be9dd21e7c0a11f887896216b53d9f2f5e52`  
		Last Modified: Fri, 27 Aug 2021 18:19:11 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c14a7793ecef764c93a3c5699156bcd2bfa499755295325b810e8fd402aae9c`  
		Last Modified: Fri, 27 Aug 2021 18:19:44 GMT  
		Size: 62.2 MB (62213151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b3a2165b82cc27fe25f781e948162fc296598212ebdb6598dbe63c0969fcb2`  
		Last Modified: Fri, 27 Aug 2021 18:19:11 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81336f3230332bdabb4dfe1ee638fc91aa3e0e3a30ca1522e74dc7fb66f6e884`  
		Last Modified: Fri, 27 Aug 2021 18:19:11 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.8.2` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:2c4312cd7ac19ad8d3f646fab632c3f216787b270a6a18d1f7e30087403fdffc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66734739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a0f97beb645a465de1903827da1dd1715e8f32b31221dabc2c35634b7db2680`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 18:10:45 GMT
ARG VAULT_VERSION=1.8.2
# Fri, 27 Aug 2021 18:10:45 GMT
# ARGS: VAULT_VERSION=1.8.2
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 27 Aug 2021 18:10:58 GMT
# ARGS: VAULT_VERSION=1.8.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 27 Aug 2021 18:10:59 GMT
# ARGS: VAULT_VERSION=1.8.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 27 Aug 2021 18:10:59 GMT
VOLUME [/vault/logs]
# Fri, 27 Aug 2021 18:10:59 GMT
VOLUME [/vault/file]
# Fri, 27 Aug 2021 18:11:00 GMT
EXPOSE 8200
# Fri, 27 Aug 2021 18:11:00 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 Aug 2021 18:11:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 18:11:00 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f0159e00faeeb7e18ca07b695f6aa7c0c0c788ea2938a30da16c3d565fca809`  
		Last Modified: Fri, 27 Aug 2021 18:11:58 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6dbcb73fcc3d448b4cae0527c0a0a96746c0a29165e8b2a17c788942be3af4`  
		Last Modified: Fri, 27 Aug 2021 18:12:07 GMT  
		Size: 64.0 MB (64019636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ce465381beed1f195d65eef219c1eb5353753fa546e311f4d2c12e88c654b0`  
		Last Modified: Fri, 27 Aug 2021 18:11:58 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f68dcec623fd3c6ec4b298f3dee3863c8f856c5b64e308ac5f8c4fe88e7d40`  
		Last Modified: Fri, 27 Aug 2021 18:11:58 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.8.2` - linux; 386

```console
$ docker pull vault@sha256:6173b34f55ee6a088350d09dbd9a27b27d773dbf1423fa85c7f22f642ee610fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68193291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56f54c3dab1d6ad7a27b37117a1f2ee6cd8398b4cbc429a485ce904d8c56392b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 17:50:42 GMT
ARG VAULT_VERSION=1.8.2
# Fri, 27 Aug 2021 17:50:42 GMT
# ARGS: VAULT_VERSION=1.8.2
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 27 Aug 2021 17:50:51 GMT
# ARGS: VAULT_VERSION=1.8.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 27 Aug 2021 17:50:53 GMT
# ARGS: VAULT_VERSION=1.8.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 27 Aug 2021 17:50:53 GMT
VOLUME [/vault/logs]
# Fri, 27 Aug 2021 17:50:53 GMT
VOLUME [/vault/file]
# Fri, 27 Aug 2021 17:50:53 GMT
EXPOSE 8200
# Fri, 27 Aug 2021 17:50:53 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 Aug 2021 17:50:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 17:50:54 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f9b5722e370732f2f325aef56a577686e0318dfbfb762492a94fb081177466`  
		Last Modified: Fri, 27 Aug 2021 17:51:55 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ba0acd6b808c25b418bbc60571d2f2098b087a293518212a4eadd14ff87ab0`  
		Last Modified: Fri, 27 Aug 2021 17:52:05 GMT  
		Size: 65.4 MB (65367161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3548486a7473383d1d7d59828ed05a69f3dd70669f08c1727c5cf0f0b491cc34`  
		Last Modified: Fri, 27 Aug 2021 17:51:54 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9401c3fa1c31d422bf103874d55c7de475021be3a6605baa0f84ab09670637a`  
		Last Modified: Fri, 27 Aug 2021 17:51:54 GMT  
		Size: 1.8 KB (1818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:latest`

```console
$ docker pull vault@sha256:1422cccf59c78e046576e84612202334d1f7d995091d33f0e00141c3b075d0db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:79c1850dfcd98a496792e87908ce5d56f9293e27fb2d0b734aede341dadd69aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.5 MB (70451820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b8a82753be914c1950b74360978eeb2c68de8550b9696f19903c9fad2a1b48c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 17:49:29 GMT
ARG VAULT_VERSION=1.8.2
# Fri, 27 Aug 2021 17:49:29 GMT
# ARGS: VAULT_VERSION=1.8.2
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 27 Aug 2021 17:49:44 GMT
# ARGS: VAULT_VERSION=1.8.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 27 Aug 2021 17:49:45 GMT
# ARGS: VAULT_VERSION=1.8.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 27 Aug 2021 17:49:45 GMT
VOLUME [/vault/logs]
# Fri, 27 Aug 2021 17:49:45 GMT
VOLUME [/vault/file]
# Fri, 27 Aug 2021 17:49:45 GMT
EXPOSE 8200
# Fri, 27 Aug 2021 17:49:46 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 Aug 2021 17:49:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 17:49:46 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985e31a6bb65ae8ae336ae741cb08cb354fc42dc6685f50b679aff4364fb8311`  
		Last Modified: Fri, 27 Aug 2021 17:50:33 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0458da6383c22ad93107f4eab8b19313efe64eae1c4aaa61d6f74ca6a14cdd5d`  
		Last Modified: Fri, 27 Aug 2021 17:50:43 GMT  
		Size: 67.6 MB (67634098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be96eae97a36426ae377bea74c0bb67bcff4559776ddb2adadb14ee92504c48`  
		Last Modified: Fri, 27 Aug 2021 17:50:33 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db08138f178f2d0dd4005b7e4550d8f43d9b99c382b91e4a2d077befd6f8f01`  
		Last Modified: Fri, 27 Aug 2021 17:50:33 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:6aebcc5b1f9eedbe7e5e72589cc09f06489cf0d8d01e9014ac01b98c0f11e7e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.8 MB (64843871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49c7f65637cae381ef8e4a74113373911a7f37433ea424c4c5c7dd87222a1ae6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 18:16:43 GMT
ARG VAULT_VERSION=1.8.2
# Fri, 27 Aug 2021 18:16:45 GMT
# ARGS: VAULT_VERSION=1.8.2
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 27 Aug 2021 18:17:06 GMT
# ARGS: VAULT_VERSION=1.8.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 27 Aug 2021 18:17:08 GMT
# ARGS: VAULT_VERSION=1.8.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 27 Aug 2021 18:17:09 GMT
VOLUME [/vault/logs]
# Fri, 27 Aug 2021 18:17:09 GMT
VOLUME [/vault/file]
# Fri, 27 Aug 2021 18:17:10 GMT
EXPOSE 8200
# Fri, 27 Aug 2021 18:17:10 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 Aug 2021 18:17:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 18:17:11 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcff2c885efceb6b909c389313f1be9dd21e7c0a11f887896216b53d9f2f5e52`  
		Last Modified: Fri, 27 Aug 2021 18:19:11 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c14a7793ecef764c93a3c5699156bcd2bfa499755295325b810e8fd402aae9c`  
		Last Modified: Fri, 27 Aug 2021 18:19:44 GMT  
		Size: 62.2 MB (62213151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b3a2165b82cc27fe25f781e948162fc296598212ebdb6598dbe63c0969fcb2`  
		Last Modified: Fri, 27 Aug 2021 18:19:11 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81336f3230332bdabb4dfe1ee638fc91aa3e0e3a30ca1522e74dc7fb66f6e884`  
		Last Modified: Fri, 27 Aug 2021 18:19:11 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:2c4312cd7ac19ad8d3f646fab632c3f216787b270a6a18d1f7e30087403fdffc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66734739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a0f97beb645a465de1903827da1dd1715e8f32b31221dabc2c35634b7db2680`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 18:10:45 GMT
ARG VAULT_VERSION=1.8.2
# Fri, 27 Aug 2021 18:10:45 GMT
# ARGS: VAULT_VERSION=1.8.2
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 27 Aug 2021 18:10:58 GMT
# ARGS: VAULT_VERSION=1.8.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 27 Aug 2021 18:10:59 GMT
# ARGS: VAULT_VERSION=1.8.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 27 Aug 2021 18:10:59 GMT
VOLUME [/vault/logs]
# Fri, 27 Aug 2021 18:10:59 GMT
VOLUME [/vault/file]
# Fri, 27 Aug 2021 18:11:00 GMT
EXPOSE 8200
# Fri, 27 Aug 2021 18:11:00 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 Aug 2021 18:11:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 18:11:00 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f0159e00faeeb7e18ca07b695f6aa7c0c0c788ea2938a30da16c3d565fca809`  
		Last Modified: Fri, 27 Aug 2021 18:11:58 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6dbcb73fcc3d448b4cae0527c0a0a96746c0a29165e8b2a17c788942be3af4`  
		Last Modified: Fri, 27 Aug 2021 18:12:07 GMT  
		Size: 64.0 MB (64019636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ce465381beed1f195d65eef219c1eb5353753fa546e311f4d2c12e88c654b0`  
		Last Modified: Fri, 27 Aug 2021 18:11:58 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f68dcec623fd3c6ec4b298f3dee3863c8f856c5b64e308ac5f8c4fe88e7d40`  
		Last Modified: Fri, 27 Aug 2021 18:11:58 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:6173b34f55ee6a088350d09dbd9a27b27d773dbf1423fa85c7f22f642ee610fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68193291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56f54c3dab1d6ad7a27b37117a1f2ee6cd8398b4cbc429a485ce904d8c56392b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 17:50:42 GMT
ARG VAULT_VERSION=1.8.2
# Fri, 27 Aug 2021 17:50:42 GMT
# ARGS: VAULT_VERSION=1.8.2
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 27 Aug 2021 17:50:51 GMT
# ARGS: VAULT_VERSION=1.8.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 27 Aug 2021 17:50:53 GMT
# ARGS: VAULT_VERSION=1.8.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 27 Aug 2021 17:50:53 GMT
VOLUME [/vault/logs]
# Fri, 27 Aug 2021 17:50:53 GMT
VOLUME [/vault/file]
# Fri, 27 Aug 2021 17:50:53 GMT
EXPOSE 8200
# Fri, 27 Aug 2021 17:50:53 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 Aug 2021 17:50:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 17:50:54 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f9b5722e370732f2f325aef56a577686e0318dfbfb762492a94fb081177466`  
		Last Modified: Fri, 27 Aug 2021 17:51:55 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ba0acd6b808c25b418bbc60571d2f2098b087a293518212a4eadd14ff87ab0`  
		Last Modified: Fri, 27 Aug 2021 17:52:05 GMT  
		Size: 65.4 MB (65367161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3548486a7473383d1d7d59828ed05a69f3dd70669f08c1727c5cf0f0b491cc34`  
		Last Modified: Fri, 27 Aug 2021 17:51:54 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9401c3fa1c31d422bf103874d55c7de475021be3a6605baa0f84ab09670637a`  
		Last Modified: Fri, 27 Aug 2021 17:51:54 GMT  
		Size: 1.8 KB (1818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
