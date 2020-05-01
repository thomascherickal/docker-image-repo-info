<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:1.3.5`](#vault135)
-	[`vault:1.4.1`](#vault141)
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

## `vault:1.4.1`

```console
$ docker pull vault@sha256:8b56a8bc7fe22379723b0313bd78668389bfa93e693c4f7d574a23d1efcab23c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.4.1` - linux; amd64

```console
$ docker pull vault@sha256:a26845ac976fa471f1a373eba30d2e7b42ddd344c9aef094fddfad091bbd9941
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52086658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c0b037d27e02c53553aed5ec2cc68a1366bd566603753a58a2fc1d84670f2dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Thu, 30 Apr 2020 23:23:02 GMT
ARG VAULT_VERSION=1.4.1
# Thu, 30 Apr 2020 23:23:03 GMT
# ARGS: VAULT_VERSION=1.4.1
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 30 Apr 2020 23:23:08 GMT
# ARGS: VAULT_VERSION=1.4.1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 30 Apr 2020 23:23:09 GMT
# ARGS: VAULT_VERSION=1.4.1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 30 Apr 2020 23:23:09 GMT
VOLUME [/vault/logs]
# Thu, 30 Apr 2020 23:23:09 GMT
VOLUME [/vault/file]
# Thu, 30 Apr 2020 23:23:09 GMT
EXPOSE 8200
# Thu, 30 Apr 2020 23:23:09 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Apr 2020 23:23:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Apr 2020 23:23:10 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeddf51eb574fe4086d95e946e882704602f6ba0674bd149b30ef12de1cfb23a`  
		Last Modified: Thu, 30 Apr 2020 23:23:21 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719720d4ff92845ca3a651e34c3194f7cfdccdc3e22b10b9d3ace6f4f4c4c7a2`  
		Last Modified: Thu, 30 Apr 2020 23:23:28 GMT  
		Size: 49.3 MB (49287841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48e6ba784e76f9523d3593d12289ae72e4d4a3df8d5cdf24e3e1f9651a1dffe`  
		Last Modified: Thu, 30 Apr 2020 23:23:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c90a552e78f344edd89162a644c100c8018d1d4886146956f7b1b5c6db145d8`  
		Last Modified: Thu, 30 Apr 2020 23:23:21 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.4.1` - linux; arm variant v6

```console
$ docker pull vault@sha256:7f34f85c6fd6e784e709b647aaf047f8d77b7124c8eb8d2838744035bbf77aa4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48750490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eccb931aa4de7946dbc4200c6018eeda9dc344407a74c3a9c0e7aba85550846`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Thu, 30 Apr 2020 22:49:36 GMT
ARG VAULT_VERSION=1.4.1
# Thu, 30 Apr 2020 22:49:39 GMT
# ARGS: VAULT_VERSION=1.4.1
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 30 Apr 2020 22:49:52 GMT
# ARGS: VAULT_VERSION=1.4.1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 30 Apr 2020 22:49:57 GMT
# ARGS: VAULT_VERSION=1.4.1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 30 Apr 2020 22:49:58 GMT
VOLUME [/vault/logs]
# Thu, 30 Apr 2020 22:49:58 GMT
VOLUME [/vault/file]
# Thu, 30 Apr 2020 22:50:00 GMT
EXPOSE 8200
# Thu, 30 Apr 2020 22:50:00 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Apr 2020 22:50:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Apr 2020 22:50:02 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bae059fb6ee383d13b76e8199fe680b670b50d3a8debd53af6dc10b77b746d2`  
		Last Modified: Thu, 30 Apr 2020 22:50:26 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be40547728495837e4d9e4dc4c6e0a0f3684d469ba6dcfbd3b90b8dfebe05e28`  
		Last Modified: Thu, 30 Apr 2020 22:50:39 GMT  
		Size: 46.2 MB (46174681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ea035ae3e8fde6c764d66e41bd3c5239c151b423090936e9bb115883127ad3`  
		Last Modified: Thu, 30 Apr 2020 22:50:25 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608a370ad5a6b7c4f9a18fa4abbb575ee1eb265cf27dcec3180fd92df6468f2a`  
		Last Modified: Thu, 30 Apr 2020 22:50:25 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.4.1` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:42a379f308523389d74c688689eb1d3fe583f2a23e443646abc16e0ff244d02f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49005666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11f257defa5e02ebb02c1d60f92c3eaeb7995671805975be855009d5abf76f34`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Thu, 30 Apr 2020 23:04:20 GMT
ARG VAULT_VERSION=1.4.1
# Thu, 30 Apr 2020 23:04:22 GMT
# ARGS: VAULT_VERSION=1.4.1
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 30 Apr 2020 23:04:30 GMT
# ARGS: VAULT_VERSION=1.4.1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 30 Apr 2020 23:04:34 GMT
# ARGS: VAULT_VERSION=1.4.1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 30 Apr 2020 23:04:35 GMT
VOLUME [/vault/logs]
# Thu, 30 Apr 2020 23:04:36 GMT
VOLUME [/vault/file]
# Thu, 30 Apr 2020 23:04:37 GMT
EXPOSE 8200
# Thu, 30 Apr 2020 23:04:38 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Apr 2020 23:04:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Apr 2020 23:04:41 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96982a74cc76586856ab6e7e5d543f558c2da73708c0f1fdc59bb818f63b1bd7`  
		Last Modified: Thu, 30 Apr 2020 23:05:00 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d869d63eeebca7f8139c9f5caa6b00fc5fbd6e56484c6a2f94c81e9d330d8c68`  
		Last Modified: Thu, 30 Apr 2020 23:05:12 GMT  
		Size: 46.3 MB (46283636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ebbaf751de7e83db075ab3e91df393ae34e5b16ccb09fdf9b703bdeed38a12`  
		Last Modified: Thu, 30 Apr 2020 23:05:00 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d31208ea685718061a5d06961466cb502eeb49da1abacc09b919f17f4736ac`  
		Last Modified: Thu, 30 Apr 2020 23:05:00 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.4.1` - linux; 386

```console
$ docker pull vault@sha256:4161adbd9733623c089bbac60cbac66c55326284baf7fb72f5781d9a56184088
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50249392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:644f771e1495603781113e0e6f57751f21a32b2387319b0d9e93493ef3750dad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Thu, 30 Apr 2020 22:38:54 GMT
ARG VAULT_VERSION=1.4.1
# Thu, 30 Apr 2020 22:38:54 GMT
# ARGS: VAULT_VERSION=1.4.1
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 30 Apr 2020 22:39:00 GMT
# ARGS: VAULT_VERSION=1.4.1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 30 Apr 2020 22:39:01 GMT
# ARGS: VAULT_VERSION=1.4.1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 30 Apr 2020 22:39:02 GMT
VOLUME [/vault/logs]
# Thu, 30 Apr 2020 22:39:02 GMT
VOLUME [/vault/file]
# Thu, 30 Apr 2020 22:39:02 GMT
EXPOSE 8200
# Thu, 30 Apr 2020 22:39:02 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Apr 2020 22:39:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Apr 2020 22:39:03 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8f140e7f5c1453257f2207c3917187ce98ae5dae62d36e045e3e3d0e88c91a0`  
		Last Modified: Thu, 30 Apr 2020 22:39:15 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1969de6153f2faae20e319a709e6ff5245277e4eb9a7c1e2b82c28bb83b0c6a`  
		Last Modified: Thu, 30 Apr 2020 22:39:24 GMT  
		Size: 47.5 MB (47459030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89573f57ae0d242b9fdb2d4360b7e900508f7229e3e77a22706c81c10477b6db`  
		Last Modified: Thu, 30 Apr 2020 22:39:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e0092dd3a81d9bc2436ae1660c854393c135bcaaceb6f939ff107085d776dd`  
		Last Modified: Thu, 30 Apr 2020 22:39:15 GMT  
		Size: 1.8 KB (1818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:latest`

```console
$ docker pull vault@sha256:8b56a8bc7fe22379723b0313bd78668389bfa93e693c4f7d574a23d1efcab23c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:a26845ac976fa471f1a373eba30d2e7b42ddd344c9aef094fddfad091bbd9941
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52086658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c0b037d27e02c53553aed5ec2cc68a1366bd566603753a58a2fc1d84670f2dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Thu, 30 Apr 2020 23:23:02 GMT
ARG VAULT_VERSION=1.4.1
# Thu, 30 Apr 2020 23:23:03 GMT
# ARGS: VAULT_VERSION=1.4.1
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 30 Apr 2020 23:23:08 GMT
# ARGS: VAULT_VERSION=1.4.1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 30 Apr 2020 23:23:09 GMT
# ARGS: VAULT_VERSION=1.4.1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 30 Apr 2020 23:23:09 GMT
VOLUME [/vault/logs]
# Thu, 30 Apr 2020 23:23:09 GMT
VOLUME [/vault/file]
# Thu, 30 Apr 2020 23:23:09 GMT
EXPOSE 8200
# Thu, 30 Apr 2020 23:23:09 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Apr 2020 23:23:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Apr 2020 23:23:10 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeddf51eb574fe4086d95e946e882704602f6ba0674bd149b30ef12de1cfb23a`  
		Last Modified: Thu, 30 Apr 2020 23:23:21 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719720d4ff92845ca3a651e34c3194f7cfdccdc3e22b10b9d3ace6f4f4c4c7a2`  
		Last Modified: Thu, 30 Apr 2020 23:23:28 GMT  
		Size: 49.3 MB (49287841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48e6ba784e76f9523d3593d12289ae72e4d4a3df8d5cdf24e3e1f9651a1dffe`  
		Last Modified: Thu, 30 Apr 2020 23:23:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c90a552e78f344edd89162a644c100c8018d1d4886146956f7b1b5c6db145d8`  
		Last Modified: Thu, 30 Apr 2020 23:23:21 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:7f34f85c6fd6e784e709b647aaf047f8d77b7124c8eb8d2838744035bbf77aa4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48750490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eccb931aa4de7946dbc4200c6018eeda9dc344407a74c3a9c0e7aba85550846`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Thu, 30 Apr 2020 22:49:36 GMT
ARG VAULT_VERSION=1.4.1
# Thu, 30 Apr 2020 22:49:39 GMT
# ARGS: VAULT_VERSION=1.4.1
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 30 Apr 2020 22:49:52 GMT
# ARGS: VAULT_VERSION=1.4.1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 30 Apr 2020 22:49:57 GMT
# ARGS: VAULT_VERSION=1.4.1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 30 Apr 2020 22:49:58 GMT
VOLUME [/vault/logs]
# Thu, 30 Apr 2020 22:49:58 GMT
VOLUME [/vault/file]
# Thu, 30 Apr 2020 22:50:00 GMT
EXPOSE 8200
# Thu, 30 Apr 2020 22:50:00 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Apr 2020 22:50:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Apr 2020 22:50:02 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bae059fb6ee383d13b76e8199fe680b670b50d3a8debd53af6dc10b77b746d2`  
		Last Modified: Thu, 30 Apr 2020 22:50:26 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be40547728495837e4d9e4dc4c6e0a0f3684d469ba6dcfbd3b90b8dfebe05e28`  
		Last Modified: Thu, 30 Apr 2020 22:50:39 GMT  
		Size: 46.2 MB (46174681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ea035ae3e8fde6c764d66e41bd3c5239c151b423090936e9bb115883127ad3`  
		Last Modified: Thu, 30 Apr 2020 22:50:25 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608a370ad5a6b7c4f9a18fa4abbb575ee1eb265cf27dcec3180fd92df6468f2a`  
		Last Modified: Thu, 30 Apr 2020 22:50:25 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:42a379f308523389d74c688689eb1d3fe583f2a23e443646abc16e0ff244d02f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49005666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11f257defa5e02ebb02c1d60f92c3eaeb7995671805975be855009d5abf76f34`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Thu, 30 Apr 2020 23:04:20 GMT
ARG VAULT_VERSION=1.4.1
# Thu, 30 Apr 2020 23:04:22 GMT
# ARGS: VAULT_VERSION=1.4.1
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 30 Apr 2020 23:04:30 GMT
# ARGS: VAULT_VERSION=1.4.1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 30 Apr 2020 23:04:34 GMT
# ARGS: VAULT_VERSION=1.4.1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 30 Apr 2020 23:04:35 GMT
VOLUME [/vault/logs]
# Thu, 30 Apr 2020 23:04:36 GMT
VOLUME [/vault/file]
# Thu, 30 Apr 2020 23:04:37 GMT
EXPOSE 8200
# Thu, 30 Apr 2020 23:04:38 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Apr 2020 23:04:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Apr 2020 23:04:41 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96982a74cc76586856ab6e7e5d543f558c2da73708c0f1fdc59bb818f63b1bd7`  
		Last Modified: Thu, 30 Apr 2020 23:05:00 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d869d63eeebca7f8139c9f5caa6b00fc5fbd6e56484c6a2f94c81e9d330d8c68`  
		Last Modified: Thu, 30 Apr 2020 23:05:12 GMT  
		Size: 46.3 MB (46283636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ebbaf751de7e83db075ab3e91df393ae34e5b16ccb09fdf9b703bdeed38a12`  
		Last Modified: Thu, 30 Apr 2020 23:05:00 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d31208ea685718061a5d06961466cb502eeb49da1abacc09b919f17f4736ac`  
		Last Modified: Thu, 30 Apr 2020 23:05:00 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:4161adbd9733623c089bbac60cbac66c55326284baf7fb72f5781d9a56184088
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50249392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:644f771e1495603781113e0e6f57751f21a32b2387319b0d9e93493ef3750dad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Thu, 30 Apr 2020 22:38:54 GMT
ARG VAULT_VERSION=1.4.1
# Thu, 30 Apr 2020 22:38:54 GMT
# ARGS: VAULT_VERSION=1.4.1
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 30 Apr 2020 22:39:00 GMT
# ARGS: VAULT_VERSION=1.4.1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 30 Apr 2020 22:39:01 GMT
# ARGS: VAULT_VERSION=1.4.1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 30 Apr 2020 22:39:02 GMT
VOLUME [/vault/logs]
# Thu, 30 Apr 2020 22:39:02 GMT
VOLUME [/vault/file]
# Thu, 30 Apr 2020 22:39:02 GMT
EXPOSE 8200
# Thu, 30 Apr 2020 22:39:02 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Apr 2020 22:39:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Apr 2020 22:39:03 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8f140e7f5c1453257f2207c3917187ce98ae5dae62d36e045e3e3d0e88c91a0`  
		Last Modified: Thu, 30 Apr 2020 22:39:15 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1969de6153f2faae20e319a709e6ff5245277e4eb9a7c1e2b82c28bb83b0c6a`  
		Last Modified: Thu, 30 Apr 2020 22:39:24 GMT  
		Size: 47.5 MB (47459030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89573f57ae0d242b9fdb2d4360b7e900508f7229e3e77a22706c81c10477b6db`  
		Last Modified: Thu, 30 Apr 2020 22:39:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e0092dd3a81d9bc2436ae1660c854393c135bcaaceb6f939ff107085d776dd`  
		Last Modified: Thu, 30 Apr 2020 22:39:15 GMT  
		Size: 1.8 KB (1818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
