<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:1.5.9`](#vault159)
-	[`vault:1.6.5`](#vault165)
-	[`vault:1.7.3`](#vault173)
-	[`vault:1.8.0-rc2`](#vault180-rc2)
-	[`vault:latest`](#vaultlatest)

## `vault:1.5.9`

```console
$ docker pull vault@sha256:82750d706fa8fb3770687c4f9aeaf1cf0b88d058601700f211d5253734dfefd6
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
$ docker pull vault@sha256:e8dbf7067b426b003cee072091a9763507b8c920ab430181143a32cc4a0d8766
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51676367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60866ad528e4397791a2bcd202baaf2a8d3207ea6cfe4ea3033994832facd388`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Thu, 15 Jul 2021 00:06:37 GMT
ARG VAULT_VERSION=1.5.9
# Thu, 15 Jul 2021 00:06:39 GMT
# ARGS: VAULT_VERSION=1.5.9
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 15 Jul 2021 00:06:51 GMT
# ARGS: VAULT_VERSION=1.5.9
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 15 Jul 2021 00:06:54 GMT
# ARGS: VAULT_VERSION=1.5.9
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 15 Jul 2021 00:06:54 GMT
VOLUME [/vault/logs]
# Thu, 15 Jul 2021 00:06:54 GMT
VOLUME [/vault/file]
# Thu, 15 Jul 2021 00:06:55 GMT
EXPOSE 8200
# Thu, 15 Jul 2021 00:06:55 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 15 Jul 2021 00:06:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jul 2021 00:06:56 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a908339bc86c73e60e82cf6df664f77c77ec4907d9cb4dc0beb243c3199890`  
		Last Modified: Thu, 15 Jul 2021 00:09:44 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0720fc9f6fc843ebb41bf2908b86dec967ff2459522128652d29b2f998e3cc0`  
		Last Modified: Thu, 15 Jul 2021 00:10:11 GMT  
		Size: 49.1 MB (49050963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67e5dab2f8ce892a2a4dd909b423a2e084020a62dc88f72403b9cbf2dc4b9a9`  
		Last Modified: Thu, 15 Jul 2021 00:09:44 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de29419b041295bba897f2d52b4aba3e7d830fcd1f2dddc3a5fe84a4a01f741b`  
		Last Modified: Thu, 15 Jul 2021 00:09:44 GMT  
		Size: 1.8 KB (1823 bytes)  
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
$ docker pull vault@sha256:eb780dd8c8888f8dbf42cff06e8cefb644912bdc0cd9278724878de875861957
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
$ docker pull vault@sha256:36012b961067da0b55268f628412d729ead7bc5081090dd7994d82559fcaf6ba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63790773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0648eb7ae2cfc84e11f0f27a6d38c559b053150c644984a4f96f1be385b0940e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Thu, 15 Jul 2021 00:06:06 GMT
ARG VAULT_VERSION=1.6.5
# Thu, 15 Jul 2021 00:06:08 GMT
# ARGS: VAULT_VERSION=1.6.5
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 15 Jul 2021 00:06:22 GMT
# ARGS: VAULT_VERSION=1.6.5
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 15 Jul 2021 00:06:24 GMT
# ARGS: VAULT_VERSION=1.6.5
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 15 Jul 2021 00:06:25 GMT
VOLUME [/vault/logs]
# Thu, 15 Jul 2021 00:06:25 GMT
VOLUME [/vault/file]
# Thu, 15 Jul 2021 00:06:26 GMT
EXPOSE 8200
# Thu, 15 Jul 2021 00:06:26 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 15 Jul 2021 00:06:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jul 2021 00:06:27 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe5b35cdc96c4dd844ee252eaf65d757622d388070eb407a2daba669a1417cd`  
		Last Modified: Thu, 15 Jul 2021 00:09:00 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fd6237276b24cc7383045652337043c4c358ce6f390c5d2ebfaf7fb5eea3dd`  
		Last Modified: Thu, 15 Jul 2021 00:09:35 GMT  
		Size: 61.2 MB (61165374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4218fcf4731bfdb420d3e539de286e359bb46a1aea34b8b7e72122c996ae6802`  
		Last Modified: Thu, 15 Jul 2021 00:09:00 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c4510a3735aab6c06912e835a275bcd8e0006c452d894d516e249fa227a933`  
		Last Modified: Thu, 15 Jul 2021 00:09:01 GMT  
		Size: 1.8 KB (1822 bytes)  
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
$ docker pull vault@sha256:6085e96fa42c2524eef7bf9af0cf5199da0b16964003b3f88e2b8195b6acb52b
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
$ docker pull vault@sha256:e41107473db771d1d507617944b827acbd2373a5d9c50e2524dfe477ad2eda47
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67780854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c73d6b58f009d6981055069c8663ce27752e37f21c734591a4f66a18a4884cc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Thu, 15 Jul 2021 00:05:35 GMT
ARG VAULT_VERSION=1.7.3
# Thu, 15 Jul 2021 00:05:37 GMT
# ARGS: VAULT_VERSION=1.7.3
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 15 Jul 2021 00:05:51 GMT
# ARGS: VAULT_VERSION=1.7.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 15 Jul 2021 00:05:53 GMT
# ARGS: VAULT_VERSION=1.7.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 15 Jul 2021 00:05:54 GMT
VOLUME [/vault/logs]
# Thu, 15 Jul 2021 00:05:54 GMT
VOLUME [/vault/file]
# Thu, 15 Jul 2021 00:05:55 GMT
EXPOSE 8200
# Thu, 15 Jul 2021 00:05:55 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 15 Jul 2021 00:05:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jul 2021 00:05:56 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d1cd8b574c76d61b2b099a7cc166d563e91d00e4202c3624a531cb407bcf92`  
		Last Modified: Thu, 15 Jul 2021 00:08:11 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4842b855836390fa47525ba05f856c17236e4febe7195d3811bbb22e527cdb41`  
		Last Modified: Thu, 15 Jul 2021 00:08:48 GMT  
		Size: 65.2 MB (65155457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fba45c3fd386e2a16021de58147e72091b15ca895820410637233b9fc1a433`  
		Last Modified: Thu, 15 Jul 2021 00:08:11 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf28e6d17fbd2d352d6276ffcaa2fc73ec077c805b1016cf43512e3bf57edad`  
		Last Modified: Thu, 15 Jul 2021 00:08:11 GMT  
		Size: 1.8 KB (1819 bytes)  
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

## `vault:1.8.0-rc2`

```console
$ docker pull vault@sha256:fbcf5916e59e2c4458023335faff539e42201a869cdd93ff9351a32a8e4cc029
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.8.0-rc2` - linux; amd64

```console
$ docker pull vault@sha256:5f3641df9ea0a4275124b6bef7321b583c91ef33ef21920ff3fc249936aa73b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68684355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bafbe3b310d0c7326b28b3f8b5bdd4d65e9edfa27eb5a12fb6db9ecc9bd14e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Jul 2021 00:20:48 GMT
ARG VAULT_VERSION=1.8.0-rc2
# Thu, 15 Jul 2021 00:20:49 GMT
# ARGS: VAULT_VERSION=1.8.0-rc2
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 15 Jul 2021 00:20:56 GMT
# ARGS: VAULT_VERSION=1.8.0-rc2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 15 Jul 2021 00:20:57 GMT
# ARGS: VAULT_VERSION=1.8.0-rc2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 15 Jul 2021 00:20:57 GMT
VOLUME [/vault/logs]
# Thu, 15 Jul 2021 00:20:57 GMT
VOLUME [/vault/file]
# Thu, 15 Jul 2021 00:20:58 GMT
EXPOSE 8200
# Thu, 15 Jul 2021 00:20:58 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 15 Jul 2021 00:20:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jul 2021 00:20:58 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b908a56f68d9e02a8e39d3b5d04b768ffac5301d8e157d292450935707897ddb`  
		Last Modified: Thu, 15 Jul 2021 00:21:17 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8086c3732d85c822b537e08a608cc2219422e5c8c0d00514dcc8903173e6feb6`  
		Last Modified: Thu, 15 Jul 2021 00:21:26 GMT  
		Size: 65.9 MB (65869114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d62461a3817dee690e3687229801cc4105938b475f4e7f16671df75eb8bdb83`  
		Last Modified: Thu, 15 Jul 2021 00:21:16 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf57fab0331ff167a2275fd52c26fe5bf7fbca034ec5e732a34ea52010d18c3f`  
		Last Modified: Thu, 15 Jul 2021 00:21:17 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.8.0-rc2` - linux; arm variant v6

```console
$ docker pull vault@sha256:4a667d0ba9826e59420f96710bb2a95dee6f5d3c45c59dd9a67408a9fa8ce825
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.3 MB (63302896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cbed4b515de8354e2cbd8a2a43a76781a45dc8a64f3a240605207b6d2ca18da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Thu, 15 Jul 2021 00:05:04 GMT
ARG VAULT_VERSION=1.8.0-rc2
# Thu, 15 Jul 2021 00:05:06 GMT
# ARGS: VAULT_VERSION=1.8.0-rc2
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 15 Jul 2021 00:05:21 GMT
# ARGS: VAULT_VERSION=1.8.0-rc2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 15 Jul 2021 00:05:23 GMT
# ARGS: VAULT_VERSION=1.8.0-rc2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 15 Jul 2021 00:05:23 GMT
VOLUME [/vault/logs]
# Thu, 15 Jul 2021 00:05:24 GMT
VOLUME [/vault/file]
# Thu, 15 Jul 2021 00:05:24 GMT
EXPOSE 8200
# Thu, 15 Jul 2021 00:05:25 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 15 Jul 2021 00:05:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jul 2021 00:05:26 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470430ecaee1f27cbcc8eede9eb2c6feeb3c26b4c220eb6af8b94830583fe228`  
		Last Modified: Thu, 15 Jul 2021 00:07:30 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4034761ef7138797ff21de7618eb660acbbf86fa53de9b5f0ffebd61a5847dc7`  
		Last Modified: Thu, 15 Jul 2021 00:08:03 GMT  
		Size: 60.7 MB (60677491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:042bb3ee7c00f32cdae394cd378b9911bfba4d9f859435ac9988752cb5c0b870`  
		Last Modified: Thu, 15 Jul 2021 00:07:29 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cfd5bb32d9407977c045326a754c9e16ecacb6a9e2771f7099f25b2325e6dbd`  
		Last Modified: Thu, 15 Jul 2021 00:07:29 GMT  
		Size: 1.8 KB (1826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.8.0-rc2` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:0f2a69fdb67d4ad522c405e53f602548f2784ed16367f12718375dfb5c5dcd45
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (65049402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a33e54bf02c7a23bc660ea1b76ce6f88aaaa5813373e08598e61fdc30aa8f80`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jul 2021 00:20:24 GMT
ARG VAULT_VERSION=1.8.0-rc2
# Thu, 15 Jul 2021 00:20:24 GMT
# ARGS: VAULT_VERSION=1.8.0-rc2
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 15 Jul 2021 00:20:34 GMT
# ARGS: VAULT_VERSION=1.8.0-rc2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 15 Jul 2021 00:20:35 GMT
# ARGS: VAULT_VERSION=1.8.0-rc2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 15 Jul 2021 00:20:35 GMT
VOLUME [/vault/logs]
# Thu, 15 Jul 2021 00:20:36 GMT
VOLUME [/vault/file]
# Thu, 15 Jul 2021 00:20:36 GMT
EXPOSE 8200
# Thu, 15 Jul 2021 00:20:36 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 15 Jul 2021 00:20:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jul 2021 00:20:37 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ecc73edafacceb3b4c9825e337a5118a8ad44130046c3d4a3ce4073b3691cc2`  
		Last Modified: Thu, 15 Jul 2021 00:21:09 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6306bf73e0c8ff1f98a1333d7adb6130d48dce82305f69653afdaf52989dacc`  
		Last Modified: Thu, 15 Jul 2021 00:21:18 GMT  
		Size: 62.3 MB (62334106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7480e23c0ef5bdc5b47b88c6226f68fb196d43e169e58e0a3ee42bacd13a2604`  
		Last Modified: Thu, 15 Jul 2021 00:21:09 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a200a0f914df324b229eacb258df9d87a56d9b37f699bd9bb11403d7e92e9d0`  
		Last Modified: Thu, 15 Jul 2021 00:21:09 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.8.0-rc2` - linux; 386

```console
$ docker pull vault@sha256:b6f6086380de094e918cc82ad872bf24e24a597fac2187dd4283767b7780778d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66513763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21905ba37de12c1deca0823c9afc359d0328e5b452b9d1924992326023f4c086`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Wed, 14 Jul 2021 23:51:33 GMT
ARG VAULT_VERSION=1.8.0-rc2
# Wed, 14 Jul 2021 23:51:34 GMT
# ARGS: VAULT_VERSION=1.8.0-rc2
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 14 Jul 2021 23:51:42 GMT
# ARGS: VAULT_VERSION=1.8.0-rc2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 14 Jul 2021 23:51:43 GMT
# ARGS: VAULT_VERSION=1.8.0-rc2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 14 Jul 2021 23:51:43 GMT
VOLUME [/vault/logs]
# Wed, 14 Jul 2021 23:51:43 GMT
VOLUME [/vault/file]
# Wed, 14 Jul 2021 23:51:44 GMT
EXPOSE 8200
# Wed, 14 Jul 2021 23:51:44 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Jul 2021 23:51:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jul 2021 23:51:44 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df532f0ab99b360283414bb88ba5174649b561dc1f6690d786dd193c2c13a5c`  
		Last Modified: Wed, 14 Jul 2021 23:52:15 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca270a56fd5b3cd7d23237a4a590d4c455c891d39a99c265baae1e1072ca6d0`  
		Last Modified: Wed, 14 Jul 2021 23:52:24 GMT  
		Size: 63.7 MB (63691598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaed1adec7fd1128bad0364d86e6d992dc2f13bd5d5a3cc074418f69f052e315`  
		Last Modified: Wed, 14 Jul 2021 23:52:15 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfd7f351bf1e1b519055dedd42445eb22a692106bb3ffdebfa9b8a159cce325`  
		Last Modified: Wed, 14 Jul 2021 23:52:15 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:latest`

```console
$ docker pull vault@sha256:6085e96fa42c2524eef7bf9af0cf5199da0b16964003b3f88e2b8195b6acb52b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

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

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:e41107473db771d1d507617944b827acbd2373a5d9c50e2524dfe477ad2eda47
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67780854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c73d6b58f009d6981055069c8663ce27752e37f21c734591a4f66a18a4884cc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Thu, 15 Jul 2021 00:05:35 GMT
ARG VAULT_VERSION=1.7.3
# Thu, 15 Jul 2021 00:05:37 GMT
# ARGS: VAULT_VERSION=1.7.3
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 15 Jul 2021 00:05:51 GMT
# ARGS: VAULT_VERSION=1.7.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 15 Jul 2021 00:05:53 GMT
# ARGS: VAULT_VERSION=1.7.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 15 Jul 2021 00:05:54 GMT
VOLUME [/vault/logs]
# Thu, 15 Jul 2021 00:05:54 GMT
VOLUME [/vault/file]
# Thu, 15 Jul 2021 00:05:55 GMT
EXPOSE 8200
# Thu, 15 Jul 2021 00:05:55 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 15 Jul 2021 00:05:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jul 2021 00:05:56 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d1cd8b574c76d61b2b099a7cc166d563e91d00e4202c3624a531cb407bcf92`  
		Last Modified: Thu, 15 Jul 2021 00:08:11 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4842b855836390fa47525ba05f856c17236e4febe7195d3811bbb22e527cdb41`  
		Last Modified: Thu, 15 Jul 2021 00:08:48 GMT  
		Size: 65.2 MB (65155457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fba45c3fd386e2a16021de58147e72091b15ca895820410637233b9fc1a433`  
		Last Modified: Thu, 15 Jul 2021 00:08:11 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf28e6d17fbd2d352d6276ffcaa2fc73ec077c805b1016cf43512e3bf57edad`  
		Last Modified: Thu, 15 Jul 2021 00:08:11 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

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

### `vault:latest` - linux; 386

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
