<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:1.3.5`](#vault135)
-	[`vault:1.4.0`](#vault140)
-	[`vault:latest`](#vaultlatest)

## `vault:1.3.5`

**does not exist** (yet?)

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
