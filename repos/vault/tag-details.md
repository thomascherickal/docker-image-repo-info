<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:1.3.5`](#vault135)
-	[`vault:1.4.0`](#vault140)
-	[`vault:latest`](#vaultlatest)

## `vault:1.3.5`

```console
$ docker pull vault@sha256:56fc96e556e8687b2fec0f49c68c9281ac654ea3a6161b74796a31e4d6107611
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.3.5` - linux; amd64

```console
$ docker pull vault@sha256:3b20593bdfaf860e9f43eeac1bd1e5128e5f2cd12b41884ebda0da3a964c64e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51677926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8d54d6686df1009d2b9ed5630d0eefab91a0352cec727bd8410e229ada27cec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Thu, 30 Apr 2020 19:40:20 GMT
ARG VAULT_VERSION=1.3.5
# Thu, 30 Apr 2020 19:40:20 GMT
# ARGS: VAULT_VERSION=1.3.5
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 30 Apr 2020 19:40:26 GMT
# ARGS: VAULT_VERSION=1.3.5
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 30 Apr 2020 19:40:26 GMT
# ARGS: VAULT_VERSION=1.3.5
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 30 Apr 2020 19:40:27 GMT
VOLUME [/vault/logs]
# Thu, 30 Apr 2020 19:40:27 GMT
VOLUME [/vault/file]
# Thu, 30 Apr 2020 19:40:27 GMT
EXPOSE 8200
# Thu, 30 Apr 2020 19:40:27 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Apr 2020 19:40:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Apr 2020 19:40:28 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99fba5e2a09ff407eae0428db95b802bd0dd4438dbb9fe7affa05296d9f79dea`  
		Last Modified: Thu, 30 Apr 2020 19:40:35 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2538bc3c97861db33ccc8b4e17f80b1e0b87676ed84ec69a6fdd95064452155`  
		Last Modified: Thu, 30 Apr 2020 19:40:45 GMT  
		Size: 48.9 MB (48879114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4478b16647f4a09837a3f528de7d6ae6cd7835100e8d716b71ecbed2186ce09`  
		Last Modified: Thu, 30 Apr 2020 19:40:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12256afa952c988894920fe1b3b0c4f29e65d804c5c96d7b4046ead6371fc455`  
		Last Modified: Thu, 30 Apr 2020 19:40:36 GMT  
		Size: 1.8 KB (1818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.3.5` - linux; arm variant v6

```console
$ docker pull vault@sha256:29d33613f1e0aea3d3daee9fc4ede6f36a66f39b2beac8395b69203d5dfc93ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48667473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e67ce65df754406abb1122e16cfc587918b4689f427597e14de9d689191ec29`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Thu, 30 Apr 2020 19:18:33 GMT
ARG VAULT_VERSION=1.3.5
# Thu, 30 Apr 2020 19:18:37 GMT
# ARGS: VAULT_VERSION=1.3.5
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 30 Apr 2020 19:18:51 GMT
# ARGS: VAULT_VERSION=1.3.5
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 30 Apr 2020 19:18:56 GMT
# ARGS: VAULT_VERSION=1.3.5
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 30 Apr 2020 19:18:57 GMT
VOLUME [/vault/logs]
# Thu, 30 Apr 2020 19:18:58 GMT
VOLUME [/vault/file]
# Thu, 30 Apr 2020 19:18:59 GMT
EXPOSE 8200
# Thu, 30 Apr 2020 19:19:00 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Apr 2020 19:19:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Apr 2020 19:19:03 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76b3d0c0aa6d352cfb36507c23f0f75b85993fc8cf532f92b864f54c06d9878`  
		Last Modified: Thu, 30 Apr 2020 19:19:24 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f897a159ace28dbb62f4c4e5e6a0232f2c4df65e27406dee8a2f600d8046c27`  
		Last Modified: Thu, 30 Apr 2020 19:19:35 GMT  
		Size: 46.1 MB (46091667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43cf97c79eb46e43360543c0e871b2a618c65d88b266a8c5bb1d71959a3dd5c`  
		Last Modified: Thu, 30 Apr 2020 19:19:25 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed5747a6c29e9547384f6c69473cd2e385243c83899133b3273e673e64652ec`  
		Last Modified: Thu, 30 Apr 2020 19:19:25 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.3.5` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:1015bd810b2e679460655badf7384bfa2124d8fac50ca58455cc77699138ef07
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48718392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:925c1458dae0ee003b92538c920a9f41afbf721c339db0d1b8e1be32335250c6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Thu, 30 Apr 2020 19:42:18 GMT
ARG VAULT_VERSION=1.3.5
# Thu, 30 Apr 2020 19:42:20 GMT
# ARGS: VAULT_VERSION=1.3.5
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 30 Apr 2020 19:42:27 GMT
# ARGS: VAULT_VERSION=1.3.5
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 30 Apr 2020 19:42:29 GMT
# ARGS: VAULT_VERSION=1.3.5
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 30 Apr 2020 19:42:30 GMT
VOLUME [/vault/logs]
# Thu, 30 Apr 2020 19:42:30 GMT
VOLUME [/vault/file]
# Thu, 30 Apr 2020 19:42:31 GMT
EXPOSE 8200
# Thu, 30 Apr 2020 19:42:31 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Apr 2020 19:42:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Apr 2020 19:42:33 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43428912bc99eaf1a5abbc848f8dc78017622ce9c52143c7e57c00f4d7c54d3a`  
		Last Modified: Thu, 30 Apr 2020 19:42:43 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d84d1d07c219b013b6d51758a39eb0c6fe8e1d30eff0a45fac26c3a27c5a269`  
		Last Modified: Thu, 30 Apr 2020 19:43:30 GMT  
		Size: 46.0 MB (45996368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528d0b7a72f8a06201da25d18f27c7a9b06c4f4fc17302510dbb565d7cc7e2cf`  
		Last Modified: Thu, 30 Apr 2020 19:42:43 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c520c4b149fbdafbd336965188f6df41b988718e12374ab29767b4c2c6ac811`  
		Last Modified: Thu, 30 Apr 2020 19:42:43 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.3.5` - linux; 386

```console
$ docker pull vault@sha256:f14406083da62be6d8e620a97e2333bdd1965e9022fc254e58d3e17d038cf87c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50127482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd7b19d54a241de8a7d90d962dc8e9372aeecb54519fe396f96e7765ce0112df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Thu, 30 Apr 2020 19:06:32 GMT
ARG VAULT_VERSION=1.3.5
# Thu, 30 Apr 2020 19:06:32 GMT
# ARGS: VAULT_VERSION=1.3.5
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 30 Apr 2020 19:06:38 GMT
# ARGS: VAULT_VERSION=1.3.5
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 30 Apr 2020 19:06:39 GMT
# ARGS: VAULT_VERSION=1.3.5
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 30 Apr 2020 19:06:40 GMT
VOLUME [/vault/logs]
# Thu, 30 Apr 2020 19:06:40 GMT
VOLUME [/vault/file]
# Thu, 30 Apr 2020 19:06:40 GMT
EXPOSE 8200
# Thu, 30 Apr 2020 19:06:40 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Apr 2020 19:06:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Apr 2020 19:06:41 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b1243a7c955357d3c28406d2aed6e11141b5a569f0c355a19db19bde6b66a4`  
		Last Modified: Thu, 30 Apr 2020 19:06:49 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5ff61da9e738c296178265f3278170863f592908de83fae26c850265946022`  
		Last Modified: Thu, 30 Apr 2020 19:07:38 GMT  
		Size: 47.3 MB (47337119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83b22cb5193395865ed84b40a21ae765cd55e9ba75ca774b3cc4832c5219dd8`  
		Last Modified: Thu, 30 Apr 2020 19:06:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a5d61895b2a850bf3585a55752fea20359eefeae28969ddaa91bf1ca642743`  
		Last Modified: Thu, 30 Apr 2020 19:06:49 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.4.0`

```console
$ docker pull vault@sha256:33908dea33cdfc33dcd730383cbab355727511d3626db5a51857904d76cdb972
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.4.0` - linux; amd64

```console
$ docker pull vault@sha256:429bd3ad2fac882cbed0684aa9d3cc52ef3ba102d8cbcb28045ef8b3fcc47776
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.0 MB (52042418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc24be06890f2556b491dbd9d62a0c70c71a8570b6105fb72fb60f39b93d67a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:34:45 GMT
ARG VAULT_VERSION=1.4.0
# Fri, 24 Apr 2020 17:34:46 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 24 Apr 2020 17:34:51 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 24 Apr 2020 17:34:52 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 24 Apr 2020 17:34:52 GMT
VOLUME [/vault/logs]
# Fri, 24 Apr 2020 17:34:52 GMT
VOLUME [/vault/file]
# Fri, 24 Apr 2020 17:34:52 GMT
EXPOSE 8200
# Fri, 24 Apr 2020 17:34:52 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 17:34:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 17:34:53 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9fb3a824964878bf19b40b234ee130c09bae9b0647f3906d8025a9384e44ce`  
		Last Modified: Fri, 24 Apr 2020 17:35:00 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6050beefa07818ca6197b6068af10e97d7d34795e7443696304b9c1746f19d62`  
		Last Modified: Fri, 24 Apr 2020 17:35:08 GMT  
		Size: 49.2 MB (49243602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b2f9bea30ff23f0f319fe4af7a6ac3e3895e0731082ee6d16575bbf935e031`  
		Last Modified: Fri, 24 Apr 2020 17:35:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a01a1ac8d9c4f06d05bc5ffb7d10c35137e7fc41ae6243a5ee6c0d52e461e8`  
		Last Modified: Fri, 24 Apr 2020 17:35:00 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.4.0` - linux; arm variant v6

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

### `vault:1.4.0` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:7d3c0003fa1a2603e619302571d4310a67f32cab68f8129e45e4e29464db2100
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48958914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aee1b32ebf5b94156bca5f6c81dd54d9ffb64b4a13f9dd02be9804541ab65872`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:48:46 GMT
ARG VAULT_VERSION=1.4.0
# Fri, 24 Apr 2020 14:48:48 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 24 Apr 2020 14:48:55 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 24 Apr 2020 14:48:57 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 24 Apr 2020 14:48:58 GMT
VOLUME [/vault/logs]
# Fri, 24 Apr 2020 14:48:58 GMT
VOLUME [/vault/file]
# Fri, 24 Apr 2020 14:48:59 GMT
EXPOSE 8200
# Fri, 24 Apr 2020 14:48:59 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:49:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:49:01 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c3bae969493a88bf7edc9ff8759393d4f7d67fcd5f5b2c35be5537df104607`  
		Last Modified: Fri, 24 Apr 2020 14:49:10 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eae976a2c758fbf2244b6ef1ee00ce746676d679bd23481247083c1d849b4ed`  
		Last Modified: Fri, 24 Apr 2020 14:49:21 GMT  
		Size: 46.2 MB (46236887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80600aacb591c1bcc8629cb7d29932f97b8fc94c62340e44caac4e217ea259eb`  
		Last Modified: Fri, 24 Apr 2020 14:49:11 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f71c941e1d30f829890d8988597cc3b2318d512e3fe6514f834740f3b1ede4a`  
		Last Modified: Fri, 24 Apr 2020 14:49:10 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.4.0` - linux; 386

```console
$ docker pull vault@sha256:b642b0e2705ae7f6f6fe389fb41689800c8b37cd52f2bb1999260af9ece653a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50191817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2af7607fa689ecf7123907d7c571217e1fdfcea819096d1c03f5d86af3bba6a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:28:31 GMT
ARG VAULT_VERSION=1.4.0
# Fri, 24 Apr 2020 04:28:31 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 24 Apr 2020 04:28:37 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 24 Apr 2020 04:28:38 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 24 Apr 2020 04:28:38 GMT
VOLUME [/vault/logs]
# Fri, 24 Apr 2020 04:28:38 GMT
VOLUME [/vault/file]
# Fri, 24 Apr 2020 04:28:39 GMT
EXPOSE 8200
# Fri, 24 Apr 2020 04:28:39 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 04:28:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:28:39 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35948ce46c9bbb639111b6f584f69db84132b9f7855c2138f559801f5c856caa`  
		Last Modified: Fri, 24 Apr 2020 04:28:46 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7e6dba2d733546db05083fc04570e2d8c1c27a9a2693900d465b27f57cdbab`  
		Last Modified: Fri, 24 Apr 2020 04:28:54 GMT  
		Size: 47.4 MB (47401455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc7f897682e1331201245e788b67b9a5f36d9a1581d44490ef1bc5d3e1972b8`  
		Last Modified: Fri, 24 Apr 2020 04:28:46 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beef6a268b07a0d3e48d8ce0a5d93331486848eb0d0834009d56245dff79283f`  
		Last Modified: Fri, 24 Apr 2020 04:28:46 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:latest`

```console
$ docker pull vault@sha256:33908dea33cdfc33dcd730383cbab355727511d3626db5a51857904d76cdb972
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:429bd3ad2fac882cbed0684aa9d3cc52ef3ba102d8cbcb28045ef8b3fcc47776
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.0 MB (52042418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc24be06890f2556b491dbd9d62a0c70c71a8570b6105fb72fb60f39b93d67a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:34:45 GMT
ARG VAULT_VERSION=1.4.0
# Fri, 24 Apr 2020 17:34:46 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 24 Apr 2020 17:34:51 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 24 Apr 2020 17:34:52 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 24 Apr 2020 17:34:52 GMT
VOLUME [/vault/logs]
# Fri, 24 Apr 2020 17:34:52 GMT
VOLUME [/vault/file]
# Fri, 24 Apr 2020 17:34:52 GMT
EXPOSE 8200
# Fri, 24 Apr 2020 17:34:52 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 17:34:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 17:34:53 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9fb3a824964878bf19b40b234ee130c09bae9b0647f3906d8025a9384e44ce`  
		Last Modified: Fri, 24 Apr 2020 17:35:00 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6050beefa07818ca6197b6068af10e97d7d34795e7443696304b9c1746f19d62`  
		Last Modified: Fri, 24 Apr 2020 17:35:08 GMT  
		Size: 49.2 MB (49243602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b2f9bea30ff23f0f319fe4af7a6ac3e3895e0731082ee6d16575bbf935e031`  
		Last Modified: Fri, 24 Apr 2020 17:35:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a01a1ac8d9c4f06d05bc5ffb7d10c35137e7fc41ae6243a5ee6c0d52e461e8`  
		Last Modified: Fri, 24 Apr 2020 17:35:00 GMT  
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
$ docker pull vault@sha256:7d3c0003fa1a2603e619302571d4310a67f32cab68f8129e45e4e29464db2100
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48958914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aee1b32ebf5b94156bca5f6c81dd54d9ffb64b4a13f9dd02be9804541ab65872`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:48:46 GMT
ARG VAULT_VERSION=1.4.0
# Fri, 24 Apr 2020 14:48:48 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 24 Apr 2020 14:48:55 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 24 Apr 2020 14:48:57 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 24 Apr 2020 14:48:58 GMT
VOLUME [/vault/logs]
# Fri, 24 Apr 2020 14:48:58 GMT
VOLUME [/vault/file]
# Fri, 24 Apr 2020 14:48:59 GMT
EXPOSE 8200
# Fri, 24 Apr 2020 14:48:59 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:49:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:49:01 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c3bae969493a88bf7edc9ff8759393d4f7d67fcd5f5b2c35be5537df104607`  
		Last Modified: Fri, 24 Apr 2020 14:49:10 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eae976a2c758fbf2244b6ef1ee00ce746676d679bd23481247083c1d849b4ed`  
		Last Modified: Fri, 24 Apr 2020 14:49:21 GMT  
		Size: 46.2 MB (46236887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80600aacb591c1bcc8629cb7d29932f97b8fc94c62340e44caac4e217ea259eb`  
		Last Modified: Fri, 24 Apr 2020 14:49:11 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f71c941e1d30f829890d8988597cc3b2318d512e3fe6514f834740f3b1ede4a`  
		Last Modified: Fri, 24 Apr 2020 14:49:10 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:b642b0e2705ae7f6f6fe389fb41689800c8b37cd52f2bb1999260af9ece653a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50191817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2af7607fa689ecf7123907d7c571217e1fdfcea819096d1c03f5d86af3bba6a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:28:31 GMT
ARG VAULT_VERSION=1.4.0
# Fri, 24 Apr 2020 04:28:31 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 24 Apr 2020 04:28:37 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 24 Apr 2020 04:28:38 GMT
# ARGS: VAULT_VERSION=1.4.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 24 Apr 2020 04:28:38 GMT
VOLUME [/vault/logs]
# Fri, 24 Apr 2020 04:28:38 GMT
VOLUME [/vault/file]
# Fri, 24 Apr 2020 04:28:39 GMT
EXPOSE 8200
# Fri, 24 Apr 2020 04:28:39 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Apr 2020 04:28:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:28:39 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35948ce46c9bbb639111b6f584f69db84132b9f7855c2138f559801f5c856caa`  
		Last Modified: Fri, 24 Apr 2020 04:28:46 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7e6dba2d733546db05083fc04570e2d8c1c27a9a2693900d465b27f57cdbab`  
		Last Modified: Fri, 24 Apr 2020 04:28:54 GMT  
		Size: 47.4 MB (47401455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc7f897682e1331201245e788b67b9a5f36d9a1581d44490ef1bc5d3e1972b8`  
		Last Modified: Fri, 24 Apr 2020 04:28:46 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beef6a268b07a0d3e48d8ce0a5d93331486848eb0d0834009d56245dff79283f`  
		Last Modified: Fri, 24 Apr 2020 04:28:46 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
