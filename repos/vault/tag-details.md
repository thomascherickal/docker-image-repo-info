<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:1.4.7`](#vault147)
-	[`vault:1.5.7`](#vault157)
-	[`vault:1.6.3`](#vault163)
-	[`vault:1.7.0-rc1`](#vault170-rc1)
-	[`vault:latest`](#vaultlatest)

## `vault:1.4.7`

```console
$ docker pull vault@sha256:d5fee23d1ab4671aaeec01752147339525ed030e3b08c1d616c791980fce7a30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.4.7` - linux; amd64

```console
$ docker pull vault@sha256:a89b032ef3fe48cd23244f20077714d30e3a3901ccd1aed36c8292497ca67191
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52081816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60f6715e7edbc90c73a28f4f654678907b90f94153778eabc1c92baa0bb00f92`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:20 GMT
ADD file:74b25a491c5eda6bdc97427d5c0f344be56370a103df816f89ef96052b79a736 in / 
# Wed, 24 Feb 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Sat, 13 Mar 2021 11:42:28 GMT
ARG VAULT_VERSION=1.4.7
# Sat, 13 Mar 2021 11:42:29 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 13 Mar 2021 11:42:34 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 13 Mar 2021 11:42:35 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 13 Mar 2021 11:42:35 GMT
VOLUME [/vault/logs]
# Sat, 13 Mar 2021 11:42:36 GMT
VOLUME [/vault/file]
# Sat, 13 Mar 2021 11:42:36 GMT
EXPOSE 8200
# Sat, 13 Mar 2021 11:42:36 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Mar 2021 11:42:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Mar 2021 11:42:36 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:8464c5956bbe86052636266c809545517fb2fbc0b945ecc9f0189d73ee1cb0c6`  
		Last Modified: Wed, 24 Feb 2021 20:20:47 GMT  
		Size: 2.8 MB (2797017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd30ca4c08dff6cf9dfc88f07b844d7cb3f2d5cb9783a92a7839556fe824e69c`  
		Last Modified: Sat, 13 Mar 2021 11:43:41 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf487472bae9299bedc12738264602bc66ff4dcd76245ae90c073bc6d4ff50e`  
		Last Modified: Sat, 13 Mar 2021 11:43:48 GMT  
		Size: 49.3 MB (49281498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9367525ae6f0aa446f88f9ef19470c8ac895f3d6d8d9edda94304dbe9db95a5b`  
		Last Modified: Sat, 13 Mar 2021 11:43:41 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca20f4a0079ac91a06fbc1e0150ba1cb131dacc8e475166b0c633bb58ac6ba9e`  
		Last Modified: Sat, 13 Mar 2021 11:43:41 GMT  
		Size: 1.8 KB (1821 bytes)  
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
$ docker pull vault@sha256:ac99c0c10f8546fc2d87ce524f4392ab2aa277491760230cde16995d0b3832ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48964643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:069d7e1b99400d2b252b1b013f79e519fd8a5007cf00732970e9151384e44b5a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 24 Feb 2021 20:40:02 GMT
ADD file:422b410b46901dfebf19c61ed06d0bc9931c018b0d96f35da99e4fc409a7776b in / 
# Wed, 24 Feb 2021 20:40:03 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 04:16:25 GMT
ARG VAULT_VERSION=1.4.7
# Thu, 25 Feb 2021 04:16:27 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 25 Feb 2021 04:16:33 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 25 Feb 2021 04:16:36 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 25 Feb 2021 04:16:37 GMT
VOLUME [/vault/logs]
# Thu, 25 Feb 2021 04:16:38 GMT
VOLUME [/vault/file]
# Thu, 25 Feb 2021 04:16:38 GMT
EXPOSE 8200
# Thu, 25 Feb 2021 04:16:39 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 25 Feb 2021 04:16:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 04:16:40 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:1287318d28f14b1b909b2cd8ff908cb037ec28d475bcdf70d1b14fdc0869650f`  
		Last Modified: Wed, 24 Feb 2021 20:40:42 GMT  
		Size: 2.7 MB (2720385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9027e395332ca8325f6a9c3b247306ea693dcadd44b9a28c0fa95a79487f7e4a`  
		Last Modified: Thu, 25 Feb 2021 04:17:43 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9938f9a801a7d4323b4ab271783cda2a32d843a5360d57d7db7f251815dcf32`  
		Last Modified: Thu, 25 Feb 2021 04:17:54 GMT  
		Size: 46.2 MB (46240962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545582878d948aeedfb9334813af75134816bd89ec1d27364fa712fe9318b681`  
		Last Modified: Thu, 25 Feb 2021 04:17:43 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bd197544029b70887df308abaee16a9adf0c2f9ce95bd02d09b9a58a210bcd`  
		Last Modified: Thu, 25 Feb 2021 04:17:43 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.4.7` - linux; 386

```console
$ docker pull vault@sha256:b9734b15de7e34fdfbf36d4ae74737bc6a646c0482a3b7c45e0f0012d948cf86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50214569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af3bb1714b76162aae8557cae08feffc09d24d9de656cd8f148f74f43ae78f66`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 24 Feb 2021 20:38:57 GMT
ADD file:b5ef4a4abd9ccb894bdda7a5750878d13fbac4746c7b173c5dc88cf4846fc976 in / 
# Wed, 24 Feb 2021 20:38:57 GMT
CMD ["/bin/sh"]
# Sat, 13 Mar 2021 04:21:13 GMT
ARG VAULT_VERSION=1.4.7
# Sat, 13 Mar 2021 04:21:14 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 13 Mar 2021 04:21:19 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 13 Mar 2021 04:21:20 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 13 Mar 2021 04:21:21 GMT
VOLUME [/vault/logs]
# Sat, 13 Mar 2021 04:21:21 GMT
VOLUME [/vault/file]
# Sat, 13 Mar 2021 04:21:21 GMT
EXPOSE 8200
# Sat, 13 Mar 2021 04:21:21 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Mar 2021 04:21:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Mar 2021 04:21:22 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:9c18aa22aceabbea5b9c3d26c1e449591c02413fb34b574d9f73520f3fea602b`  
		Last Modified: Wed, 24 Feb 2021 20:39:36 GMT  
		Size: 2.8 MB (2788780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:337893333af33b7612c5297b9225634941437572144978bd22f18d2cb3725b66`  
		Last Modified: Sat, 13 Mar 2021 04:22:42 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4faabe768828e04b61961b8c59ef0ad38c7278efea3d06e24ff88b284e31e9a1`  
		Last Modified: Sat, 13 Mar 2021 04:22:50 GMT  
		Size: 47.4 MB (47422488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0f265f3ac02602c89f81e9a183afdd5b082e05a7ab47a6e5f0b11834b7146b`  
		Last Modified: Sat, 13 Mar 2021 04:22:42 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb123cff4479d664b63b79d0b6b5f522991288d081474ec8cef3313a77127df4`  
		Last Modified: Sat, 13 Mar 2021 04:22:42 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.5.7`

```console
$ docker pull vault@sha256:fceea51b84295260ca01b54c62e826ab94ebd948325754fe5a588b1ae174919a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.5.7` - linux; amd64

```console
$ docker pull vault@sha256:0d432dcf65f44e0f016cae1204b1288dd7abef69e9f2b7ad9576bdcb4cc3f664
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55009870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:157b357d8fcf4c9458ced7f2794403d3fd22d72960fc07fc56655c667a0331ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:20 GMT
ADD file:74b25a491c5eda6bdc97427d5c0f344be56370a103df816f89ef96052b79a736 in / 
# Wed, 24 Feb 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Sat, 13 Mar 2021 11:42:16 GMT
ARG VAULT_VERSION=1.5.7
# Sat, 13 Mar 2021 11:42:17 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 13 Mar 2021 11:42:23 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 13 Mar 2021 11:42:24 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 13 Mar 2021 11:42:24 GMT
VOLUME [/vault/logs]
# Sat, 13 Mar 2021 11:42:24 GMT
VOLUME [/vault/file]
# Sat, 13 Mar 2021 11:42:25 GMT
EXPOSE 8200
# Sat, 13 Mar 2021 11:42:25 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Mar 2021 11:42:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Mar 2021 11:42:25 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:8464c5956bbe86052636266c809545517fb2fbc0b945ecc9f0189d73ee1cb0c6`  
		Last Modified: Wed, 24 Feb 2021 20:20:47 GMT  
		Size: 2.8 MB (2797017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de17785539ac576a2cf3d68939a23c71304aa2cfbc5a77d4b2e1b052715359c`  
		Last Modified: Sat, 13 Mar 2021 11:43:26 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5823fdfb1a3721121a16fa4d1b944c44dd95c1214ed33b11fc1575d0b98792eb`  
		Last Modified: Sat, 13 Mar 2021 11:43:34 GMT  
		Size: 52.2 MB (52209554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b988c42b81ff1287b664336ff578557420df5d074685677b17ebd067acc6328`  
		Last Modified: Sat, 13 Mar 2021 11:43:26 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de8e2c6fd3368d4a6f1ecf2af491d45f677454c34be044e731cf2beb40e0716`  
		Last Modified: Sat, 13 Mar 2021 11:43:26 GMT  
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
$ docker pull vault@sha256:aed9a19f1a7ebae87e4d59d6f382004b88dcd850ad528bf6fa4f7f84b11dc861
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51918023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c10f48753ca2a05d1005e5e97ea9a7a04f55222819690bb333618761c4fa0107`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 24 Feb 2021 20:40:02 GMT
ADD file:422b410b46901dfebf19c61ed06d0bc9931c018b0d96f35da99e4fc409a7776b in / 
# Wed, 24 Feb 2021 20:40:03 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 04:16:01 GMT
ARG VAULT_VERSION=1.5.7
# Thu, 25 Feb 2021 04:16:03 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 25 Feb 2021 04:16:10 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 25 Feb 2021 04:16:13 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 25 Feb 2021 04:16:13 GMT
VOLUME [/vault/logs]
# Thu, 25 Feb 2021 04:16:14 GMT
VOLUME [/vault/file]
# Thu, 25 Feb 2021 04:16:15 GMT
EXPOSE 8200
# Thu, 25 Feb 2021 04:16:15 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 25 Feb 2021 04:16:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 04:16:17 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:1287318d28f14b1b909b2cd8ff908cb037ec28d475bcdf70d1b14fdc0869650f`  
		Last Modified: Wed, 24 Feb 2021 20:40:42 GMT  
		Size: 2.7 MB (2720385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6bdcf98a8f33143f5380d0058503d12cc6756895d54dfc775a763b88c78dc8`  
		Last Modified: Thu, 25 Feb 2021 04:17:25 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94001555867ee89de33f77cfee4e8addd014546bcfd60387cab94b4b2d87925`  
		Last Modified: Thu, 25 Feb 2021 04:17:35 GMT  
		Size: 49.2 MB (49194343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59dcfbce7fcf49406ad4b08a13dcf3ac7282b364a18a5cd4836e7a2939ca42b`  
		Last Modified: Thu, 25 Feb 2021 04:17:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499619716c039e9345346edb8a71b33536d86ef5b173f95aa5e5c04ef6729bbf`  
		Last Modified: Thu, 25 Feb 2021 04:17:25 GMT  
		Size: 1.8 KB (1818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.5.7` - linux; 386

```console
$ docker pull vault@sha256:46ec7cff4a3647c7ed489046f426ebb024642a65b2b488dd6bb135af2406311a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53087311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bad025aee0d1bd6e8b224dc8e9bbd13d122bc9d524335dac1b2fca064f5677c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 24 Feb 2021 20:38:57 GMT
ADD file:b5ef4a4abd9ccb894bdda7a5750878d13fbac4746c7b173c5dc88cf4846fc976 in / 
# Wed, 24 Feb 2021 20:38:57 GMT
CMD ["/bin/sh"]
# Sat, 13 Mar 2021 04:20:56 GMT
ARG VAULT_VERSION=1.5.7
# Sat, 13 Mar 2021 04:20:57 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 13 Mar 2021 04:21:05 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 13 Mar 2021 04:21:06 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 13 Mar 2021 04:21:06 GMT
VOLUME [/vault/logs]
# Sat, 13 Mar 2021 04:21:06 GMT
VOLUME [/vault/file]
# Sat, 13 Mar 2021 04:21:07 GMT
EXPOSE 8200
# Sat, 13 Mar 2021 04:21:07 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Mar 2021 04:21:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Mar 2021 04:21:07 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:9c18aa22aceabbea5b9c3d26c1e449591c02413fb34b574d9f73520f3fea602b`  
		Last Modified: Wed, 24 Feb 2021 20:39:36 GMT  
		Size: 2.8 MB (2788780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559f9e16e7b8a03f75f8d44cea6686c77a35f318e8500965d38b07e88147859c`  
		Last Modified: Sat, 13 Mar 2021 04:22:25 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f80a6539f1ecb5411831cd6d6c8e76943562b479d9bec0c0b0cbeab429b370`  
		Last Modified: Sat, 13 Mar 2021 04:22:33 GMT  
		Size: 50.3 MB (50295231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d435c9d37a5cf8cbd51d97d0ef73326f25172f8e04116c7cb74fb449ada6f728`  
		Last Modified: Sat, 13 Mar 2021 04:22:25 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e2db9573d3e2d3a763721a2b69e3eeac4c1954fab91290b331175bbf1a4ae3`  
		Last Modified: Sat, 13 Mar 2021 04:22:25 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.6.3`

```console
$ docker pull vault@sha256:17e587f3475d67cca24451848bd0ea69989fe48c18eee226d3a48db3b6aa44f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.6.3` - linux; amd64

```console
$ docker pull vault@sha256:8ef538af66967e784a7b0b32efa8c6473365194c81c3a5d717e831dd5cab9155
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (68982863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83d03b2b783e9a59abae959dd6e6c7a5ccaf9f0cf9793d8efa5ee9d699170ed3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Sat, 13 Mar 2021 11:42:02 GMT
ARG VAULT_VERSION=1.6.3
# Sat, 13 Mar 2021 11:42:03 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 13 Mar 2021 11:42:10 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 13 Mar 2021 11:42:11 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 13 Mar 2021 11:42:11 GMT
VOLUME [/vault/logs]
# Sat, 13 Mar 2021 11:42:11 GMT
VOLUME [/vault/file]
# Sat, 13 Mar 2021 11:42:12 GMT
EXPOSE 8200
# Sat, 13 Mar 2021 11:42:12 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Mar 2021 11:42:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Mar 2021 11:42:12 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf90fe65cc1210aaa1cb21c2ef7e703360fbc3ca31c3d62f2662764c3c32138`  
		Last Modified: Sat, 13 Mar 2021 11:43:07 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479c1be4a4052222497832548909cb2f5f71983ed9657a6d65499427be8f371f`  
		Last Modified: Sat, 13 Mar 2021 11:43:16 GMT  
		Size: 66.2 MB (66167936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8987a40e7560c149aebe107febfac483c7e83c593647f782b9521255bd60fdd6`  
		Last Modified: Sat, 13 Mar 2021 11:43:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982296b02bf83c568505556c537de0f55e3a951c2c000aa06ed179200bfcb8ac`  
		Last Modified: Sat, 13 Mar 2021 11:43:06 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.6.3` - linux; arm variant v6

```console
$ docker pull vault@sha256:c259ca51167c63aa9607d919b2c55db9eb7b7a78f71e451da595a562e7481760
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.7 MB (63718893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b12efd0b4318752f6ee120b58288113977130db7a2d1859621b3130c6c5e1c96`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Tue, 02 Mar 2021 23:14:53 GMT
ARG VAULT_VERSION=1.6.3
# Tue, 02 Mar 2021 23:14:54 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 02 Mar 2021 23:15:06 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 02 Mar 2021 23:15:09 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 02 Mar 2021 23:15:10 GMT
VOLUME [/vault/logs]
# Tue, 02 Mar 2021 23:15:11 GMT
VOLUME [/vault/file]
# Tue, 02 Mar 2021 23:15:12 GMT
EXPOSE 8200
# Tue, 02 Mar 2021 23:15:12 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 02 Mar 2021 23:15:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Mar 2021 23:15:14 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565cbb62e6435fa12e134fa98dd06c89e72cb48235f763bc4d730d144cc7a1f8`  
		Last Modified: Tue, 02 Mar 2021 23:15:36 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284162887dd90cdadae098858307a49f9d62bdd19a07dd1c13918486d4713703`  
		Last Modified: Tue, 02 Mar 2021 23:15:52 GMT  
		Size: 61.1 MB (61093587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b4c9ad70bb6e855693e16c1a7108c23673a58ff4897b17b3b19282ec14ed02`  
		Last Modified: Tue, 02 Mar 2021 23:15:36 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51322c75e1e50cf02683375fbc23aa2288d8dd6af7d4a84029a7c142f4749ad5`  
		Last Modified: Tue, 02 Mar 2021 23:15:36 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.6.3` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:f6f42cfae7bb0e4db405930b85246960388b493598296e32216006a25895b490
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (65015972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9db3e6d5cd58d59e467cc2628643c5c49080a729b8a28c047f4a3361fe0610ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Tue, 02 Mar 2021 23:00:04 GMT
ARG VAULT_VERSION=1.6.3
# Tue, 02 Mar 2021 23:00:07 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 02 Mar 2021 23:00:21 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 02 Mar 2021 23:00:24 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 02 Mar 2021 23:00:25 GMT
VOLUME [/vault/logs]
# Tue, 02 Mar 2021 23:00:25 GMT
VOLUME [/vault/file]
# Tue, 02 Mar 2021 23:00:27 GMT
EXPOSE 8200
# Tue, 02 Mar 2021 23:00:28 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 02 Mar 2021 23:00:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Mar 2021 23:00:30 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f28d5e0abd1f586bd1f92372c7bd965218df4b3388ea881f7c0ea48f134c4ac`  
		Last Modified: Tue, 02 Mar 2021 23:00:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea3d060932ea51ab17f91ef330c219bb2e6c99bd2db6454b557d401c15438d0`  
		Last Modified: Tue, 02 Mar 2021 23:01:12 GMT  
		Size: 62.3 MB (62301132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8efb2df7982195004f1be44691579ab5fc37954dcf8ae84a6520904e417fcf`  
		Last Modified: Tue, 02 Mar 2021 23:01:00 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7243d4f0f132c177a143c28a1854bdbf7911defe968cee4f4235698bad712b`  
		Last Modified: Tue, 02 Mar 2021 23:01:00 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.6.3` - linux; 386

```console
$ docker pull vault@sha256:c88f2267f674e946cda289fe4ca74e08b020df367d5794079ddb5697993507ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (67033174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb4690e8d201f8da8e9156bc6aaddd0fd70be06fbc0e104f51f449199ec53f7f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 17 Feb 2021 21:38:34 GMT
ADD file:eaee53da3c87749799de55809e4a5b526c56855332b961a85b1184c660f1d65b in / 
# Wed, 17 Feb 2021 21:38:35 GMT
CMD ["/bin/sh"]
# Sat, 13 Mar 2021 04:20:39 GMT
ARG VAULT_VERSION=1.6.3
# Sat, 13 Mar 2021 04:20:39 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 13 Mar 2021 04:20:47 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 13 Mar 2021 04:20:48 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 13 Mar 2021 04:20:48 GMT
VOLUME [/vault/logs]
# Sat, 13 Mar 2021 04:20:49 GMT
VOLUME [/vault/file]
# Sat, 13 Mar 2021 04:20:49 GMT
EXPOSE 8200
# Sat, 13 Mar 2021 04:20:49 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Mar 2021 04:20:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Mar 2021 04:20:49 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:86205afa28f6bc624469015a543d16608258d2828411a92c662f4fdc6d276e18`  
		Last Modified: Wed, 17 Feb 2021 21:39:07 GMT  
		Size: 2.8 MB (2818177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4e2efb828c20a20c7e10f0e0d5ad91c51d9d287e583c699ea0f71c618ad24c`  
		Last Modified: Sat, 13 Mar 2021 04:22:02 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ede3b452c48602c7f834022bf8eb76e66acb650c25659a3a2502346ffa46af6`  
		Last Modified: Sat, 13 Mar 2021 04:22:12 GMT  
		Size: 64.2 MB (64211731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb4bcc937a3d8ed95c0cfac11c12b349557d4d0b78e6bb5f26c116549971c58`  
		Last Modified: Sat, 13 Mar 2021 04:22:02 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23fcb17f032c6add01d605cca0b8b53a075bafff6cd254c40eca88402865fc4`  
		Last Modified: Sat, 13 Mar 2021 04:22:02 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.7.0-rc1`

```console
$ docker pull vault@sha256:7f4a98be2449a6bd66f6c4549bfbc29b972270c540ade0633a63499c13077c6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.7.0-rc1` - linux; amd64

```console
$ docker pull vault@sha256:a8a5a2eb133646c24e01e10ebada432ea31f6f33096013910b8f1c2a519d2877
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72670574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0fbb02843bdb085c6560a647c44f4d0ee495fe41bd7d7546d31f7ab0b9ea169`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Sat, 13 Mar 2021 11:41:49 GMT
ARG VAULT_VERSION=1.7.0-rc1
# Sat, 13 Mar 2021 11:41:50 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 13 Mar 2021 11:41:57 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 13 Mar 2021 11:41:58 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 13 Mar 2021 11:41:58 GMT
VOLUME [/vault/logs]
# Sat, 13 Mar 2021 11:41:58 GMT
VOLUME [/vault/file]
# Sat, 13 Mar 2021 11:41:59 GMT
EXPOSE 8200
# Sat, 13 Mar 2021 11:41:59 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Mar 2021 11:41:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Mar 2021 11:41:59 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d189708bdf7d1a3a66d32523fdfb5b0cb95e7b6eee69f2de65794c3536e0bee`  
		Last Modified: Sat, 13 Mar 2021 11:42:49 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75114a4435fed327213aa63951b6d29358dd66b5e5837b08dd0b8a682ae774e5`  
		Last Modified: Sat, 13 Mar 2021 11:42:59 GMT  
		Size: 69.9 MB (69855652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c92cb2e735b785be22bfe594d01f06b63210b7177bd9049f427c17e4811013`  
		Last Modified: Sat, 13 Mar 2021 11:42:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78da6e37dc8afbb172731935ddf62a41585bf819ac4be000657df1bdd9873a31`  
		Last Modified: Sat, 13 Mar 2021 11:42:49 GMT  
		Size: 1.8 KB (1818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.7.0-rc1` - linux; arm variant v6

```console
$ docker pull vault@sha256:3774e40967516f02b0e1e95c0d6d5b2a0f5d2c1fc1b1444d925b9324ef08c5d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66701202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a076fb7281763a43289d7998affb280220ace610d2111bd206b4cffd71dddf0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Fri, 12 Mar 2021 21:06:53 GMT
ARG VAULT_VERSION=1.7.0-rc1
# Fri, 12 Mar 2021 21:06:55 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 12 Mar 2021 21:07:07 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 12 Mar 2021 21:07:10 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 12 Mar 2021 21:07:11 GMT
VOLUME [/vault/logs]
# Fri, 12 Mar 2021 21:07:11 GMT
VOLUME [/vault/file]
# Fri, 12 Mar 2021 21:07:12 GMT
EXPOSE 8200
# Fri, 12 Mar 2021 21:07:13 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 12 Mar 2021 21:07:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 21:07:14 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da71943561a84c5a71b50584dce69c1fa92edeb892379413a3ca6aee79713b9f`  
		Last Modified: Fri, 12 Mar 2021 21:07:42 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd520100b4e569f3cc80cfa37639845a4acc36da813548a31e3d7e49b1f4a5d`  
		Last Modified: Fri, 12 Mar 2021 21:08:00 GMT  
		Size: 64.1 MB (64075893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7976f00f5bc42016b9f92eb0d013b94a23414c0d0c735630b236efe68d961e`  
		Last Modified: Fri, 12 Mar 2021 21:07:42 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4fd12f56f70b0f61bc421d11e7f15e4ae533e2783e397cca3dd0c1d60a1371e`  
		Last Modified: Fri, 12 Mar 2021 21:07:42 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.7.0-rc1` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:ed73bb9f084c89b67a88c4bfed7ec11a11db1410044c962b6f084a3db0feb11a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68499991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80ce08985774ad184476cafc190dac159b6f7322ef9b1ca966b0ab60fff18943`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Sat, 13 Mar 2021 06:25:45 GMT
ARG VAULT_VERSION=1.7.0-rc1
# Sat, 13 Mar 2021 06:25:49 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 13 Mar 2021 06:25:59 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 13 Mar 2021 06:26:02 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 13 Mar 2021 06:26:03 GMT
VOLUME [/vault/logs]
# Sat, 13 Mar 2021 06:26:04 GMT
VOLUME [/vault/file]
# Sat, 13 Mar 2021 06:26:05 GMT
EXPOSE 8200
# Sat, 13 Mar 2021 06:26:06 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Mar 2021 06:26:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Mar 2021 06:26:08 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c614c25a2a603e767ba7d983e8eddc8390d54163c3e747a9a2aedcbc60ac50a7`  
		Last Modified: Sat, 13 Mar 2021 06:26:36 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960530f4d600b44ba58f3965d809d4ccddd978461b56b8c11c4fefc5382b4b9c`  
		Last Modified: Sat, 13 Mar 2021 06:26:52 GMT  
		Size: 65.8 MB (65785148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0f8143ef809ca5941b3cb951bb433f30aa769ec38501eeb5a88e99413c969d`  
		Last Modified: Sat, 13 Mar 2021 06:26:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c013fd21fca75b8d62d3b591ec23c30af5237fc4ba49c5ccc4604574df5bb6cd`  
		Last Modified: Sat, 13 Mar 2021 06:26:36 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.7.0-rc1` - linux; 386

```console
$ docker pull vault@sha256:33d8485e41ee4bc1644a2594a96629156686db055178a5a8cf725f557e3b20fe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.5 MB (70535213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97b9d341d2c791e479ceae1b24a791fe4f60a658fd97d8df9b70abad4bd8b2f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 17 Feb 2021 21:38:34 GMT
ADD file:eaee53da3c87749799de55809e4a5b526c56855332b961a85b1184c660f1d65b in / 
# Wed, 17 Feb 2021 21:38:35 GMT
CMD ["/bin/sh"]
# Sat, 13 Mar 2021 04:20:22 GMT
ARG VAULT_VERSION=1.7.0-rc1
# Sat, 13 Mar 2021 04:20:23 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 13 Mar 2021 04:20:31 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 13 Mar 2021 04:20:32 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 13 Mar 2021 04:20:33 GMT
VOLUME [/vault/logs]
# Sat, 13 Mar 2021 04:20:33 GMT
VOLUME [/vault/file]
# Sat, 13 Mar 2021 04:20:33 GMT
EXPOSE 8200
# Sat, 13 Mar 2021 04:20:33 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Mar 2021 04:20:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Mar 2021 04:20:34 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:86205afa28f6bc624469015a543d16608258d2828411a92c662f4fdc6d276e18`  
		Last Modified: Wed, 17 Feb 2021 21:39:07 GMT  
		Size: 2.8 MB (2818177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec077617e334124628bc315a2fac18f3a58ea03e5b9a27f0c5b4b47d12ff901`  
		Last Modified: Sat, 13 Mar 2021 04:21:41 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a971e165b52bc71c746279bbbb38b15b3d7719f28c73fc1e73085ff029adf55`  
		Last Modified: Sat, 13 Mar 2021 04:21:53 GMT  
		Size: 67.7 MB (67713774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9d35fbfd3611ce6411fa0ddcf21074c6cb74465db84181af0251e7ce3d9f21`  
		Last Modified: Sat, 13 Mar 2021 04:21:41 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5adcd7a014010274a71e984d64d721e11fb533558cde40d9daa5c0eb38d98f85`  
		Last Modified: Sat, 13 Mar 2021 04:21:41 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:latest`

```console
$ docker pull vault@sha256:17e587f3475d67cca24451848bd0ea69989fe48c18eee226d3a48db3b6aa44f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:8ef538af66967e784a7b0b32efa8c6473365194c81c3a5d717e831dd5cab9155
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (68982863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83d03b2b783e9a59abae959dd6e6c7a5ccaf9f0cf9793d8efa5ee9d699170ed3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Sat, 13 Mar 2021 11:42:02 GMT
ARG VAULT_VERSION=1.6.3
# Sat, 13 Mar 2021 11:42:03 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 13 Mar 2021 11:42:10 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 13 Mar 2021 11:42:11 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 13 Mar 2021 11:42:11 GMT
VOLUME [/vault/logs]
# Sat, 13 Mar 2021 11:42:11 GMT
VOLUME [/vault/file]
# Sat, 13 Mar 2021 11:42:12 GMT
EXPOSE 8200
# Sat, 13 Mar 2021 11:42:12 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Mar 2021 11:42:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Mar 2021 11:42:12 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf90fe65cc1210aaa1cb21c2ef7e703360fbc3ca31c3d62f2662764c3c32138`  
		Last Modified: Sat, 13 Mar 2021 11:43:07 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479c1be4a4052222497832548909cb2f5f71983ed9657a6d65499427be8f371f`  
		Last Modified: Sat, 13 Mar 2021 11:43:16 GMT  
		Size: 66.2 MB (66167936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8987a40e7560c149aebe107febfac483c7e83c593647f782b9521255bd60fdd6`  
		Last Modified: Sat, 13 Mar 2021 11:43:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982296b02bf83c568505556c537de0f55e3a951c2c000aa06ed179200bfcb8ac`  
		Last Modified: Sat, 13 Mar 2021 11:43:06 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:c259ca51167c63aa9607d919b2c55db9eb7b7a78f71e451da595a562e7481760
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.7 MB (63718893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b12efd0b4318752f6ee120b58288113977130db7a2d1859621b3130c6c5e1c96`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Tue, 02 Mar 2021 23:14:53 GMT
ARG VAULT_VERSION=1.6.3
# Tue, 02 Mar 2021 23:14:54 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 02 Mar 2021 23:15:06 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 02 Mar 2021 23:15:09 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 02 Mar 2021 23:15:10 GMT
VOLUME [/vault/logs]
# Tue, 02 Mar 2021 23:15:11 GMT
VOLUME [/vault/file]
# Tue, 02 Mar 2021 23:15:12 GMT
EXPOSE 8200
# Tue, 02 Mar 2021 23:15:12 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 02 Mar 2021 23:15:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Mar 2021 23:15:14 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565cbb62e6435fa12e134fa98dd06c89e72cb48235f763bc4d730d144cc7a1f8`  
		Last Modified: Tue, 02 Mar 2021 23:15:36 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284162887dd90cdadae098858307a49f9d62bdd19a07dd1c13918486d4713703`  
		Last Modified: Tue, 02 Mar 2021 23:15:52 GMT  
		Size: 61.1 MB (61093587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b4c9ad70bb6e855693e16c1a7108c23673a58ff4897b17b3b19282ec14ed02`  
		Last Modified: Tue, 02 Mar 2021 23:15:36 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51322c75e1e50cf02683375fbc23aa2288d8dd6af7d4a84029a7c142f4749ad5`  
		Last Modified: Tue, 02 Mar 2021 23:15:36 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:f6f42cfae7bb0e4db405930b85246960388b493598296e32216006a25895b490
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (65015972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9db3e6d5cd58d59e467cc2628643c5c49080a729b8a28c047f4a3361fe0610ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Tue, 02 Mar 2021 23:00:04 GMT
ARG VAULT_VERSION=1.6.3
# Tue, 02 Mar 2021 23:00:07 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 02 Mar 2021 23:00:21 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 02 Mar 2021 23:00:24 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 02 Mar 2021 23:00:25 GMT
VOLUME [/vault/logs]
# Tue, 02 Mar 2021 23:00:25 GMT
VOLUME [/vault/file]
# Tue, 02 Mar 2021 23:00:27 GMT
EXPOSE 8200
# Tue, 02 Mar 2021 23:00:28 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 02 Mar 2021 23:00:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Mar 2021 23:00:30 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f28d5e0abd1f586bd1f92372c7bd965218df4b3388ea881f7c0ea48f134c4ac`  
		Last Modified: Tue, 02 Mar 2021 23:00:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea3d060932ea51ab17f91ef330c219bb2e6c99bd2db6454b557d401c15438d0`  
		Last Modified: Tue, 02 Mar 2021 23:01:12 GMT  
		Size: 62.3 MB (62301132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8efb2df7982195004f1be44691579ab5fc37954dcf8ae84a6520904e417fcf`  
		Last Modified: Tue, 02 Mar 2021 23:01:00 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7243d4f0f132c177a143c28a1854bdbf7911defe968cee4f4235698bad712b`  
		Last Modified: Tue, 02 Mar 2021 23:01:00 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:c88f2267f674e946cda289fe4ca74e08b020df367d5794079ddb5697993507ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (67033174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb4690e8d201f8da8e9156bc6aaddd0fd70be06fbc0e104f51f449199ec53f7f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 17 Feb 2021 21:38:34 GMT
ADD file:eaee53da3c87749799de55809e4a5b526c56855332b961a85b1184c660f1d65b in / 
# Wed, 17 Feb 2021 21:38:35 GMT
CMD ["/bin/sh"]
# Sat, 13 Mar 2021 04:20:39 GMT
ARG VAULT_VERSION=1.6.3
# Sat, 13 Mar 2021 04:20:39 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 13 Mar 2021 04:20:47 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 13 Mar 2021 04:20:48 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 13 Mar 2021 04:20:48 GMT
VOLUME [/vault/logs]
# Sat, 13 Mar 2021 04:20:49 GMT
VOLUME [/vault/file]
# Sat, 13 Mar 2021 04:20:49 GMT
EXPOSE 8200
# Sat, 13 Mar 2021 04:20:49 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Mar 2021 04:20:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Mar 2021 04:20:49 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:86205afa28f6bc624469015a543d16608258d2828411a92c662f4fdc6d276e18`  
		Last Modified: Wed, 17 Feb 2021 21:39:07 GMT  
		Size: 2.8 MB (2818177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4e2efb828c20a20c7e10f0e0d5ad91c51d9d287e583c699ea0f71c618ad24c`  
		Last Modified: Sat, 13 Mar 2021 04:22:02 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ede3b452c48602c7f834022bf8eb76e66acb650c25659a3a2502346ffa46af6`  
		Last Modified: Sat, 13 Mar 2021 04:22:12 GMT  
		Size: 64.2 MB (64211731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb4bcc937a3d8ed95c0cfac11c12b349557d4d0b78e6bb5f26c116549971c58`  
		Last Modified: Sat, 13 Mar 2021 04:22:02 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23fcb17f032c6add01d605cca0b8b53a075bafff6cd254c40eca88402865fc4`  
		Last Modified: Sat, 13 Mar 2021 04:22:02 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
