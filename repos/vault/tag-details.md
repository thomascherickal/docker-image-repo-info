<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:1.5.9`](#vault159)
-	[`vault:1.6.5`](#vault165)
-	[`vault:1.7.3`](#vault173)
-	[`vault:1.8.1`](#vault181)
-	[`vault:latest`](#vaultlatest)

## `vault:1.5.9`

```console
$ docker pull vault@sha256:a0ab4d91e2956f29ebe5be622aa3305a80cec31043488b150b0b76fd334e7b75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.5.9` - linux; amd64

```console
$ docker pull vault@sha256:26d722b908478e14ef06734d8076a82345d7f406247591bef23468809182a1bc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.1 MB (55099145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4810aaad94a754b1d668f1496dbac027599887b9cf9681e3073c1c36d1589d18`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Tue, 25 May 2021 00:21:50 GMT
ARG VAULT_VERSION=1.5.9
# Tue, 25 May 2021 00:21:51 GMT
# ARGS: VAULT_VERSION=1.5.9
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 25 May 2021 00:21:57 GMT
# ARGS: VAULT_VERSION=1.5.9
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 25 May 2021 00:21:58 GMT
# ARGS: VAULT_VERSION=1.5.9
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 25 May 2021 00:21:58 GMT
VOLUME [/vault/logs]
# Tue, 25 May 2021 00:21:59 GMT
VOLUME [/vault/file]
# Tue, 25 May 2021 00:21:59 GMT
EXPOSE 8200
# Tue, 25 May 2021 00:21:59 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 25 May 2021 00:21:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 May 2021 00:22:00 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7110a2d455fc9b0af555cc569995882849b4a738e647a40d6e8b0498cc5de0`  
		Last Modified: Tue, 25 May 2021 00:22:48 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b98d53fdc42a9a75062d573e3cd54c50d89b252493c09c8749570005aef42e1`  
		Last Modified: Tue, 25 May 2021 00:22:55 GMT  
		Size: 52.3 MB (52283909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae574f7e1810ceed158729b50444071e004a4ca81ee97f7d3773f660ca23e3f`  
		Last Modified: Tue, 25 May 2021 00:22:48 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cfe0a7a042084f24fe6bb6b2815b8c30295f0e3179518eb3b18b0ce7ba100c`  
		Last Modified: Tue, 25 May 2021 00:22:48 GMT  
		Size: 1.8 KB (1820 bytes)  
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
$ docker pull vault@sha256:0ca6e895e08a0ac27c58865823e2b33678807a1578957c172897c844a4de0b81
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53172659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:820ed155b380c22f413033c922bec31f0a564f0389c76bda55acc1f966c55291`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Tue, 25 May 2021 00:40:15 GMT
ARG VAULT_VERSION=1.5.9
# Tue, 25 May 2021 00:40:16 GMT
# ARGS: VAULT_VERSION=1.5.9
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 25 May 2021 00:40:23 GMT
# ARGS: VAULT_VERSION=1.5.9
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 25 May 2021 00:40:23 GMT
# ARGS: VAULT_VERSION=1.5.9
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 25 May 2021 00:40:24 GMT
VOLUME [/vault/logs]
# Tue, 25 May 2021 00:40:24 GMT
VOLUME [/vault/file]
# Tue, 25 May 2021 00:40:24 GMT
EXPOSE 8200
# Tue, 25 May 2021 00:40:24 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 25 May 2021 00:40:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 May 2021 00:40:25 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8d02c5d56208483caa02b677be5d220d197ba232c9e5de916ea50c1784f2f1`  
		Last Modified: Tue, 25 May 2021 00:41:19 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b69e3c32b0077b45fdb243b34b2f1695a6ff245a5bdb9a3a2c111d4b7b470a`  
		Last Modified: Tue, 25 May 2021 00:41:26 GMT  
		Size: 50.4 MB (50350492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e321c7e7f5d504de1afd22df040f13b5621f043a5e60e0954d243d2dc876589f`  
		Last Modified: Tue, 25 May 2021 00:41:19 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03d4118eab638fb782fcc82d2cf4942d5f19ea0d3f972a72334e49ea09a7a7d`  
		Last Modified: Tue, 25 May 2021 00:41:19 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.6.5`

```console
$ docker pull vault@sha256:1dd8e88b919b2ddf9b9b687fb4f856cb80b6c5c3fed0b0ee1427932be3ee28b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.6.5` - linux; amd64

```console
$ docker pull vault@sha256:9276f2126078769b3934416941c4741e46be56e45973cb85ec84853d14767303
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69050282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:247449edbd28cefb29d778bffaad659b3180c7b6664e9bd69f4701a624c4ff10`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Tue, 25 May 2021 00:21:37 GMT
ARG VAULT_VERSION=1.6.5
# Tue, 25 May 2021 00:21:38 GMT
# ARGS: VAULT_VERSION=1.6.5
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 25 May 2021 00:21:44 GMT
# ARGS: VAULT_VERSION=1.6.5
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 25 May 2021 00:21:46 GMT
# ARGS: VAULT_VERSION=1.6.5
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 25 May 2021 00:21:46 GMT
VOLUME [/vault/logs]
# Tue, 25 May 2021 00:21:46 GMT
VOLUME [/vault/file]
# Tue, 25 May 2021 00:21:46 GMT
EXPOSE 8200
# Tue, 25 May 2021 00:21:47 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 25 May 2021 00:21:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 May 2021 00:21:47 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c1a0fd9fba71315805cc8a1fd3d5a776dddb0e355b83f0217dcf2801d8f2b9`  
		Last Modified: Tue, 25 May 2021 00:22:31 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1956096c8a7d7a0ba03c72f5123d3d46edea112a83fc5d6ab4be8223d8ff4b93`  
		Last Modified: Tue, 25 May 2021 00:22:40 GMT  
		Size: 66.2 MB (66235046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8419dc31fa3da93f845d1f2372449f5d27379454730919251e66c992aa5ef6d7`  
		Last Modified: Tue, 25 May 2021 00:22:31 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f469972ebfb7aac47daf3413dcf4dd53169a82be734288e9a4c5ff897288b6`  
		Last Modified: Tue, 25 May 2021 00:22:31 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.6.5` - linux; arm variant v6

```console
$ docker pull vault@sha256:88660113f593e3f6ebfb0e41d6021c14112f9ac2cc96547db426df1d69e0ad01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63790777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac40a1e6f635cc74c77f6a30b7b62eee39dbf946aae3ae643075b6986cc92dc2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 30 Jul 2021 17:49:55 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Fri, 30 Jul 2021 17:49:55 GMT
CMD ["/bin/sh"]
# Sat, 31 Jul 2021 07:22:13 GMT
ARG VAULT_VERSION=1.6.5
# Sat, 31 Jul 2021 07:22:15 GMT
# ARGS: VAULT_VERSION=1.6.5
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 31 Jul 2021 07:22:31 GMT
# ARGS: VAULT_VERSION=1.6.5
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 31 Jul 2021 07:22:33 GMT
# ARGS: VAULT_VERSION=1.6.5
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 31 Jul 2021 07:22:34 GMT
VOLUME [/vault/logs]
# Sat, 31 Jul 2021 07:22:34 GMT
VOLUME [/vault/file]
# Sat, 31 Jul 2021 07:22:35 GMT
EXPOSE 8200
# Sat, 31 Jul 2021 07:22:35 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 31 Jul 2021 07:22:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 31 Jul 2021 07:22:36 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f437173d98a66bda7910c537fbcc81590352b68a23d45c7144ba1597483af0`  
		Last Modified: Sat, 31 Jul 2021 07:25:12 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906e7e97863d0a046275f1273e093770dcf1b247d827fe3b46af60c60ceb3fec`  
		Last Modified: Sat, 31 Jul 2021 07:25:44 GMT  
		Size: 61.2 MB (61165377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91187ae278ec90c6bb66820f07d0968c712146cb06924cb0445ba3d889693f2`  
		Last Modified: Sat, 31 Jul 2021 07:25:12 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558fa46196b2b227ef92eabb4a58aac1e503d6c5dc82369e121fa081875a37ff`  
		Last Modified: Sat, 31 Jul 2021 07:25:12 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.6.5` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:09a9799f52424cbcb1c6061830c5c1b412e689f95213831ec21f22f9bee5303a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.1 MB (65099505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3516e51932f2f37972e99297d352c31a55267c265efeeaf771e9e4c263f641eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:15:37 GMT
ARG VAULT_VERSION=1.6.5
# Wed, 16 Jun 2021 11:15:37 GMT
# ARGS: VAULT_VERSION=1.6.5
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 16 Jun 2021 11:15:44 GMT
# ARGS: VAULT_VERSION=1.6.5
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 16 Jun 2021 11:15:45 GMT
# ARGS: VAULT_VERSION=1.6.5
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 16 Jun 2021 11:15:45 GMT
VOLUME [/vault/logs]
# Wed, 16 Jun 2021 11:15:45 GMT
VOLUME [/vault/file]
# Wed, 16 Jun 2021 11:15:45 GMT
EXPOSE 8200
# Wed, 16 Jun 2021 11:15:45 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 16 Jun 2021 11:15:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:15:46 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb5b3df36f508fb54fb8df1b24a2127520114c3f3a34939f1afa37cfd8d347c`  
		Last Modified: Wed, 16 Jun 2021 11:16:39 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167dec37a4ac9bb7a5d60d563595fcc486b27c9bb2d8e7278f008e80b333eac9`  
		Last Modified: Wed, 16 Jun 2021 11:16:49 GMT  
		Size: 62.4 MB (62384210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670c9b6354cd7703271d8450b930f0c4aef6d74ea8132f044c313d7ec1ebce52`  
		Last Modified: Wed, 16 Jun 2021 11:16:39 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5643b6c6ea1b7554a39b75ad20de7389f6f72336f7651b0f7db128c7fb7020`  
		Last Modified: Wed, 16 Jun 2021 11:16:39 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.6.5` - linux; 386

```console
$ docker pull vault@sha256:8857732acfb260ead53f4d868720e7d391197ac85d7f378a89ffe324ad386fa0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67106549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af6abac981c5de403ead8b0a3314cbee5c638bd872d0b68789ff0eea47300a38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Tue, 25 May 2021 00:39:59 GMT
ARG VAULT_VERSION=1.6.5
# Tue, 25 May 2021 00:40:00 GMT
# ARGS: VAULT_VERSION=1.6.5
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 25 May 2021 00:40:07 GMT
# ARGS: VAULT_VERSION=1.6.5
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 25 May 2021 00:40:08 GMT
# ARGS: VAULT_VERSION=1.6.5
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 25 May 2021 00:40:08 GMT
VOLUME [/vault/logs]
# Tue, 25 May 2021 00:40:09 GMT
VOLUME [/vault/file]
# Tue, 25 May 2021 00:40:09 GMT
EXPOSE 8200
# Tue, 25 May 2021 00:40:09 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 25 May 2021 00:40:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 May 2021 00:40:09 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0a53728a931ad0904ece16168d41d8f0c40f3bd0c475a495d514fd5b7543eb`  
		Last Modified: Tue, 25 May 2021 00:41:01 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3329a03f27bbd4ceb4d9212edf53073b65e3a3dfc05c94371f3a7f9ddce0060a`  
		Last Modified: Tue, 25 May 2021 00:41:11 GMT  
		Size: 64.3 MB (64284385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4952a55250519c8ae5c5a0418bb8787c6f314d3d231d70995697ad175855e3d`  
		Last Modified: Tue, 25 May 2021 00:41:01 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895053fba6b1efc7947846e40d84e30822eeef579c6fc5f08f3043a7eb03ff81`  
		Last Modified: Tue, 25 May 2021 00:41:01 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.7.3`

```console
$ docker pull vault@sha256:55d8cb0a995c0e4a4426b9f00c8944583700edb35917d2d950ed9b2379e61830
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.7.3` - linux; amd64

```console
$ docker pull vault@sha256:53e509aaa6f72c54418b2f65f23fdd8a5ddd22bf6521c4b5bf82a8ae4edd0e53
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73952123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97ff3bfe78c3fde94206fe27d3ff7f65afa21c717949daf0e1530e8d080ca692`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 22:41:56 GMT
ARG VAULT_VERSION=1.7.3
# Wed, 16 Jun 2021 22:41:57 GMT
# ARGS: VAULT_VERSION=1.7.3
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 16 Jun 2021 22:42:03 GMT
# ARGS: VAULT_VERSION=1.7.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 16 Jun 2021 22:42:05 GMT
# ARGS: VAULT_VERSION=1.7.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 16 Jun 2021 22:42:05 GMT
VOLUME [/vault/logs]
# Wed, 16 Jun 2021 22:42:05 GMT
VOLUME [/vault/file]
# Wed, 16 Jun 2021 22:42:05 GMT
EXPOSE 8200
# Wed, 16 Jun 2021 22:42:06 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 16 Jun 2021 22:42:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 22:42:06 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01b10d36ffd7a377a9873b735fd8dad565ebf846b257ab7b600c70be268ca31`  
		Last Modified: Wed, 16 Jun 2021 22:42:41 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6b9f118d4b3b1b2b1a9515f5ca1752cf228f685e09cbcd2c2051c0f20eaac9`  
		Last Modified: Wed, 16 Jun 2021 22:42:54 GMT  
		Size: 71.1 MB (71136887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c43fa2ed89cf46209a719787b1d3eefcdfa123f226b8c54160623fe943aa9b1`  
		Last Modified: Wed, 16 Jun 2021 22:42:40 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc11702906449b2fc5c6306541b38d377e03847856a24866c235fcd5688c911c`  
		Last Modified: Wed, 16 Jun 2021 22:42:41 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.7.3` - linux; arm variant v6

```console
$ docker pull vault@sha256:e946f8b65ad2be8c4c71a365c60ce270a23423273154250617d2c27504b5d758
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67780832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12ac47fb7e244543a5b3ec851e0b7b4d68325a1ed963a7f689fc91fdfcb7336d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 30 Jul 2021 17:49:55 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Fri, 30 Jul 2021 17:49:55 GMT
CMD ["/bin/sh"]
# Sat, 31 Jul 2021 07:21:37 GMT
ARG VAULT_VERSION=1.7.3
# Sat, 31 Jul 2021 07:21:39 GMT
# ARGS: VAULT_VERSION=1.7.3
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 31 Jul 2021 07:21:56 GMT
# ARGS: VAULT_VERSION=1.7.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 31 Jul 2021 07:21:59 GMT
# ARGS: VAULT_VERSION=1.7.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 31 Jul 2021 07:21:59 GMT
VOLUME [/vault/logs]
# Sat, 31 Jul 2021 07:22:00 GMT
VOLUME [/vault/file]
# Sat, 31 Jul 2021 07:22:00 GMT
EXPOSE 8200
# Sat, 31 Jul 2021 07:22:00 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 31 Jul 2021 07:22:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 31 Jul 2021 07:22:01 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc411bce9e9b87b60981e60482bdd9e4f25fb148555ed8de27feb6aac6a3772`  
		Last Modified: Sat, 31 Jul 2021 07:24:25 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476585dbe98dd52d3a5ce9282b6e3df8a54d0231f5324766b454bd0e27bc08ce`  
		Last Modified: Sat, 31 Jul 2021 07:24:59 GMT  
		Size: 65.2 MB (65155428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e553ebd6a061651fe9ac171ddffe2afae5270d1da1b3e2b246d3c0a56f1b1e5`  
		Last Modified: Sat, 31 Jul 2021 07:24:25 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3798dbfb463d15d0aebef76e92fce3b4da92318892ce481d11e96daa7860556`  
		Last Modified: Sat, 31 Jul 2021 07:24:25 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.7.3` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:e6fa25ca5c11786f4546cc092eeb5b38d1d20e079105afac21234b3f4466a4ed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69754151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53c6317af23c62b0d73f3b9cfcddf22bb91e84fcb6b4977dc8bc2abe16d2e67f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 21:46:15 GMT
ARG VAULT_VERSION=1.7.3
# Wed, 16 Jun 2021 21:46:16 GMT
# ARGS: VAULT_VERSION=1.7.3
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 16 Jun 2021 21:46:22 GMT
# ARGS: VAULT_VERSION=1.7.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 16 Jun 2021 21:46:23 GMT
# ARGS: VAULT_VERSION=1.7.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 16 Jun 2021 21:46:23 GMT
VOLUME [/vault/logs]
# Wed, 16 Jun 2021 21:46:23 GMT
VOLUME [/vault/file]
# Wed, 16 Jun 2021 21:46:23 GMT
EXPOSE 8200
# Wed, 16 Jun 2021 21:46:24 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 16 Jun 2021 21:46:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 21:46:24 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d51d353d4c93682b1aa78d23f09bff7fffbe31e64dd314128bcdeaaf80ea7a9`  
		Last Modified: Wed, 16 Jun 2021 21:47:08 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2243a76d9dead0c9c0092b795c3db3fd5529bba9a61babc961ec80e9fd3acd`  
		Last Modified: Wed, 16 Jun 2021 21:47:19 GMT  
		Size: 67.0 MB (67038854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1dd5fd2c24e9a9adeb920170cf02d4968cbbc01c36c566464c134ff5c141f7f`  
		Last Modified: Wed, 16 Jun 2021 21:47:08 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4a667af5aa3ca6e2179f9897636a395cf45720d1deea0dcaa932885bcc3133`  
		Last Modified: Wed, 16 Jun 2021 21:47:08 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.7.3` - linux; 386

```console
$ docker pull vault@sha256:3ce2bf600b86a63a2ae838ed1efb47df5a9369bd288ece1a713a8c3b377eca2f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.8 MB (71814243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f819efa5e28c44953dd940d4ae32f6f0fa7c0fd433b64180e0a7d99dcf046d29`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 21:43:14 GMT
ARG VAULT_VERSION=1.7.3
# Wed, 16 Jun 2021 21:43:14 GMT
# ARGS: VAULT_VERSION=1.7.3
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 16 Jun 2021 21:43:22 GMT
# ARGS: VAULT_VERSION=1.7.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 16 Jun 2021 21:43:23 GMT
# ARGS: VAULT_VERSION=1.7.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 16 Jun 2021 21:43:23 GMT
VOLUME [/vault/logs]
# Wed, 16 Jun 2021 21:43:23 GMT
VOLUME [/vault/file]
# Wed, 16 Jun 2021 21:43:23 GMT
EXPOSE 8200
# Wed, 16 Jun 2021 21:43:24 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 16 Jun 2021 21:43:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 21:43:24 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a08160fcc4382ffc786991ba5c6e9c73ef0ce8ecd1a03a383e5715094a7bce5`  
		Last Modified: Wed, 16 Jun 2021 21:44:08 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3187804c6ef10e3e6f5a034f4f6951f49f56602661cfaf8face271f1d10ff888`  
		Last Modified: Wed, 16 Jun 2021 21:44:18 GMT  
		Size: 69.0 MB (68992078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a733586cbca4b00da42022f6c25c1d4c84773ae3f3f4bc47de5a6fa71380dd9f`  
		Last Modified: Wed, 16 Jun 2021 21:44:08 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5676fd992e5ea6197157bac4c55695d334e0707f5246f7cae0cf41234cd882b`  
		Last Modified: Wed, 16 Jun 2021 21:44:08 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.8.1`

**does not exist** (yet?)

## `vault:latest`

```console
$ docker pull vault@sha256:67bd14848505aac2d62354fb412ed62b17a84869ce5568d868986b21f7ae3c8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:d35855569d87911f396bf951104ff6603ca1858ef2283719a935f8bcf9167e64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68684496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2dd7a0251c2fc1283466f894f4c684cef7db165383aa8a9d1f73ccb1a55ae5c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 29 Jul 2021 00:26:24 GMT
ARG VAULT_VERSION=1.8.0
# Thu, 29 Jul 2021 00:26:25 GMT
# ARGS: VAULT_VERSION=1.8.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 29 Jul 2021 00:26:31 GMT
# ARGS: VAULT_VERSION=1.8.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 29 Jul 2021 00:26:32 GMT
# ARGS: VAULT_VERSION=1.8.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 29 Jul 2021 00:26:33 GMT
VOLUME [/vault/logs]
# Thu, 29 Jul 2021 00:26:33 GMT
VOLUME [/vault/file]
# Thu, 29 Jul 2021 00:26:33 GMT
EXPOSE 8200
# Thu, 29 Jul 2021 00:26:33 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 29 Jul 2021 00:26:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:26:34 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0007abbaf5bfc9c9d53e8d081449c32c1f4828c7837727deb632027de05b6d8b`  
		Last Modified: Thu, 29 Jul 2021 00:26:53 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c023e4795b37f3764324f309c48609f9fca8602a919d722a3a76775b9b1a6c3`  
		Last Modified: Thu, 29 Jul 2021 00:27:01 GMT  
		Size: 65.9 MB (65869257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d44eacb94ab14e9e908ac2d7f0be09ec101ef52d79188d46cc61e65679b517c`  
		Last Modified: Thu, 29 Jul 2021 00:26:53 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79331dd3afa692b3b8ab598ecf7413f6aaac834d866235379bcc60f2a6ca9e6b`  
		Last Modified: Thu, 29 Jul 2021 00:26:53 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:341b0798757dc763a28d922ec1473829ae7a986425452571f48cb89b5382cb23
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.3 MB (63301974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cf226f9e860291fb9a5de0b44d92304d0be4e6eff49a5ef0c8910040118ca17`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 30 Jul 2021 17:49:55 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Fri, 30 Jul 2021 17:49:55 GMT
CMD ["/bin/sh"]
# Sat, 31 Jul 2021 07:21:04 GMT
ARG VAULT_VERSION=1.8.0
# Sat, 31 Jul 2021 07:21:06 GMT
# ARGS: VAULT_VERSION=1.8.0
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 31 Jul 2021 07:21:21 GMT
# ARGS: VAULT_VERSION=1.8.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 31 Jul 2021 07:21:23 GMT
# ARGS: VAULT_VERSION=1.8.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 31 Jul 2021 07:21:24 GMT
VOLUME [/vault/logs]
# Sat, 31 Jul 2021 07:21:24 GMT
VOLUME [/vault/file]
# Sat, 31 Jul 2021 07:21:25 GMT
EXPOSE 8200
# Sat, 31 Jul 2021 07:21:25 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 31 Jul 2021 07:21:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 31 Jul 2021 07:21:26 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fda6cd68a2a7e0312ca39dcf86a7058e19a1bb62742bbeff8b3eab049d790e`  
		Last Modified: Sat, 31 Jul 2021 07:23:40 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542f59689c99228e12186f5530e2a6754ff5bff9fbc91fbe9f58abf998d29cf3`  
		Last Modified: Sat, 31 Jul 2021 07:24:12 GMT  
		Size: 60.7 MB (60676572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3fe215004a8876d1b930d944a69481a5b130e7dc5dc4794791475130ed259e`  
		Last Modified: Sat, 31 Jul 2021 07:23:40 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c16788d13206c3ddf23f92d51dd955794672bf56e745283147cc109f6ad730c`  
		Last Modified: Sat, 31 Jul 2021 07:23:41 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:55a623072bf1180634467be4590f127c59e64aee1c7848395be4db92d79dd2f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (65045959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66a45a645c3067d9b1c922e77730e82ec1202caeaf6ccd3af4497020c614363d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Thu, 29 Jul 2021 01:15:55 GMT
ARG VAULT_VERSION=1.8.0
# Thu, 29 Jul 2021 01:15:56 GMT
# ARGS: VAULT_VERSION=1.8.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 29 Jul 2021 01:16:03 GMT
# ARGS: VAULT_VERSION=1.8.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 29 Jul 2021 01:16:03 GMT
# ARGS: VAULT_VERSION=1.8.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 29 Jul 2021 01:16:04 GMT
VOLUME [/vault/logs]
# Thu, 29 Jul 2021 01:16:04 GMT
VOLUME [/vault/file]
# Thu, 29 Jul 2021 01:16:04 GMT
EXPOSE 8200
# Thu, 29 Jul 2021 01:16:04 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 29 Jul 2021 01:16:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jul 2021 01:16:05 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde3220e49d2ce8bdba2eb5970489a8dc1a3bb42a68a5503a4ea2c36c70299fd`  
		Last Modified: Thu, 29 Jul 2021 01:16:35 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfe9ebc842a0597b407c0b92b597f41630e20095f266b0ca719ee07fe22a734`  
		Last Modified: Thu, 29 Jul 2021 01:16:44 GMT  
		Size: 62.3 MB (62330669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6d07e431b4ac907ec2e4f61e3ca483d3627312ca8ec96c341f6375de8a3ae8`  
		Last Modified: Thu, 29 Jul 2021 01:16:35 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4477144ae1b4053c33d6dca1baa6ca018bf813cb59bb92f261a75beb35e32b57`  
		Last Modified: Thu, 29 Jul 2021 01:16:35 GMT  
		Size: 1.8 KB (1818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:8c06871a7af53c1a2d04569f8a4578a5355b0c5d24a8370ee440e8b4d1aea51e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66521424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:701d3792c7c5d19773cee42443e5db43de9d160df990b2923615aaffb636860c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 29 Jul 2021 00:38:57 GMT
ARG VAULT_VERSION=1.8.0
# Thu, 29 Jul 2021 00:38:58 GMT
# ARGS: VAULT_VERSION=1.8.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 29 Jul 2021 00:39:07 GMT
# ARGS: VAULT_VERSION=1.8.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 29 Jul 2021 00:39:08 GMT
# ARGS: VAULT_VERSION=1.8.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 29 Jul 2021 00:39:08 GMT
VOLUME [/vault/logs]
# Thu, 29 Jul 2021 00:39:09 GMT
VOLUME [/vault/file]
# Thu, 29 Jul 2021 00:39:09 GMT
EXPOSE 8200
# Thu, 29 Jul 2021 00:39:09 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 29 Jul 2021 00:39:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:39:10 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181c4c257ce65383669c0b8f3f6a86b1786310e2d42cd39161fa192fbfac28b7`  
		Last Modified: Thu, 29 Jul 2021 00:39:41 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7645e99d6d18057a084220c052baf9ff6812bf036c1365424366c0400e02c5`  
		Last Modified: Thu, 29 Jul 2021 00:39:51 GMT  
		Size: 63.7 MB (63699259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c20f9a4e638149a62395073f9d90c67dba2eddfc8af9b0ea2921b97edc90587`  
		Last Modified: Thu, 29 Jul 2021 00:39:41 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0510577c3ae1e1071acfeab3bff07332ad70b51dff10fb1c9994b5afca72c2`  
		Last Modified: Thu, 29 Jul 2021 00:39:41 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
