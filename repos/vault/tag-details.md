<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:1.3.7`](#vault137)
-	[`vault:1.4.3`](#vault143)
-	[`vault:1.5.0-rc`](#vault150-rc)
-	[`vault:latest`](#vaultlatest)

## `vault:1.3.7`

```console
$ docker pull vault@sha256:ac6010df269466eafcc12b2d01d72768a78861b7b5809cdf071070bc3aede4a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.3.7` - linux; amd64

```console
$ docker pull vault@sha256:acc05b25bfeb68766274d9ad7ed77efb33dbcb4dabe839dc5fd1e95736317a2b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51655281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a8bf6c22306e5e9088b5ecaa3cecb68fba775558461aa4eb73f3c77022d8853`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 03 Jul 2020 17:20:25 GMT
ARG VAULT_VERSION=1.3.7
# Fri, 03 Jul 2020 17:20:26 GMT
# ARGS: VAULT_VERSION=1.3.7
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 03 Jul 2020 17:20:30 GMT
# ARGS: VAULT_VERSION=1.3.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 03 Jul 2020 17:20:31 GMT
# ARGS: VAULT_VERSION=1.3.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 03 Jul 2020 17:20:31 GMT
VOLUME [/vault/logs]
# Fri, 03 Jul 2020 17:20:32 GMT
VOLUME [/vault/file]
# Fri, 03 Jul 2020 17:20:32 GMT
EXPOSE 8200
# Fri, 03 Jul 2020 17:20:32 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 03 Jul 2020 17:20:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Jul 2020 17:20:32 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94c98ff007a6228e527b75c930e0dc8c36bc836887019a4995b3d0f6c3a595e`  
		Last Modified: Fri, 03 Jul 2020 17:20:52 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb6e60c1cd20990291edd836b2afedd9969ed058ee04e69f1deb82b8da74426`  
		Last Modified: Fri, 03 Jul 2020 17:20:59 GMT  
		Size: 48.9 MB (48856460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77fc250760e0bc0f180296f0d589e7a9aa97660f52d942491e09a5829a7952e`  
		Last Modified: Fri, 03 Jul 2020 17:20:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae009c6e713de7e09ff00d44b24495c71c5956a5d46cb25b1bb8d0cdb87347e`  
		Last Modified: Fri, 03 Jul 2020 17:20:52 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.3.7` - linux; arm variant v6

```console
$ docker pull vault@sha256:f7a2b4263c950478f59d45b099085372f0fc907590fdef06aeb0cd163cf797aa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48654233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:749fe7a278eb0af5ed33e67132d82d3d47dd371d53ace899305df710f96cc972`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Fri, 03 Jul 2020 16:51:09 GMT
ARG VAULT_VERSION=1.3.7
# Fri, 03 Jul 2020 16:51:10 GMT
# ARGS: VAULT_VERSION=1.3.7
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 03 Jul 2020 16:51:20 GMT
# ARGS: VAULT_VERSION=1.3.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 03 Jul 2020 16:51:22 GMT
# ARGS: VAULT_VERSION=1.3.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 03 Jul 2020 16:51:23 GMT
VOLUME [/vault/logs]
# Fri, 03 Jul 2020 16:51:23 GMT
VOLUME [/vault/file]
# Fri, 03 Jul 2020 16:51:24 GMT
EXPOSE 8200
# Fri, 03 Jul 2020 16:51:25 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 03 Jul 2020 16:51:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Jul 2020 16:51:26 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e105b739d3ef940013db5c2871b980d1804d9b83fbf73120794e9da84162ddd`  
		Last Modified: Fri, 03 Jul 2020 16:51:57 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f336292832a8b31cbe68a1c420c2da4e3fe523cad6c3fab87a3ee2ec6022153`  
		Last Modified: Fri, 03 Jul 2020 16:52:10 GMT  
		Size: 46.1 MB (46078421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd66e375b32fbdec68b617eaae083540ac282258556ad9cce4e3a74146bb687e`  
		Last Modified: Fri, 03 Jul 2020 16:51:56 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec6e83869de8b01b38c938c3db33e7a22b0f44e936b54621848dc2c1dd54a40`  
		Last Modified: Fri, 03 Jul 2020 16:51:57 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.3.7` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:b07918d383f98e8ecea2692fc77fb59587258520596c845f20e34921c6863019
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48700679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6accbefcaa8928046c27e30e5bb680dd1103f6d010669ba1adbd6fc3bafcf76`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 03 Jul 2020 17:44:09 GMT
ARG VAULT_VERSION=1.3.7
# Fri, 03 Jul 2020 17:44:11 GMT
# ARGS: VAULT_VERSION=1.3.7
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 03 Jul 2020 17:44:18 GMT
# ARGS: VAULT_VERSION=1.3.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 03 Jul 2020 17:44:20 GMT
# ARGS: VAULT_VERSION=1.3.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 03 Jul 2020 17:44:21 GMT
VOLUME [/vault/logs]
# Fri, 03 Jul 2020 17:44:21 GMT
VOLUME [/vault/file]
# Fri, 03 Jul 2020 17:44:22 GMT
EXPOSE 8200
# Fri, 03 Jul 2020 17:44:22 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 03 Jul 2020 17:44:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Jul 2020 17:44:24 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f497a10cd55da16b299063036f64365a98533e3f359d5d2cec451768e87cb62a`  
		Last Modified: Fri, 03 Jul 2020 17:45:05 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336fed8be620784dab835b96a2e3f55c4520cd9814fc2e06c94e66fab21eafa7`  
		Last Modified: Fri, 03 Jul 2020 17:45:18 GMT  
		Size: 46.0 MB (45978649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc72b632a2b1b143481a9c861999a58829e99b2152723059cbe7c7365bbd585`  
		Last Modified: Fri, 03 Jul 2020 17:45:05 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9610512de2054f535a2e74797063a99a79f50925fde98cfb61c881a8306516b9`  
		Last Modified: Fri, 03 Jul 2020 17:45:05 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.3.7` - linux; 386

```console
$ docker pull vault@sha256:ba95a340c6a926aa63c6579f3266ba76cdebc4304261d5d0b4265f8b3fef1b1a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50105756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2706eab7b4500db8e01a165269440d2f1c34301d629d546da54e0e2be4c6149c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Fri, 03 Jul 2020 17:38:51 GMT
ARG VAULT_VERSION=1.3.7
# Fri, 03 Jul 2020 17:38:52 GMT
# ARGS: VAULT_VERSION=1.3.7
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 03 Jul 2020 17:38:58 GMT
# ARGS: VAULT_VERSION=1.3.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 03 Jul 2020 17:38:59 GMT
# ARGS: VAULT_VERSION=1.3.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 03 Jul 2020 17:38:59 GMT
VOLUME [/vault/logs]
# Fri, 03 Jul 2020 17:38:59 GMT
VOLUME [/vault/file]
# Fri, 03 Jul 2020 17:38:59 GMT
EXPOSE 8200
# Fri, 03 Jul 2020 17:39:00 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 03 Jul 2020 17:39:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Jul 2020 17:39:00 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d84e1aa7b658a04455f21055889b4ad9e13ead35c26b13658fe71a13a99bcd`  
		Last Modified: Fri, 03 Jul 2020 17:39:19 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c465b2697d2ec3867639f8f99fec5d185196dd3cfef9d2d691807e01069af6`  
		Last Modified: Fri, 03 Jul 2020 17:39:34 GMT  
		Size: 47.3 MB (47315387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727391569ad175978f87731c28df72842c7b06d86dbd83353ff4414013fa5c83`  
		Last Modified: Fri, 03 Jul 2020 17:39:19 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b02502dee475ffea4eedd293b06d56c15f483b287795ef74df8e8a30d3a1ef3`  
		Last Modified: Fri, 03 Jul 2020 17:39:20 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.4.3`

```console
$ docker pull vault@sha256:be3a63905b4d78d6e7c24fc9aacb30621d7a8a1ad8e8baff286a4ba110db16e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.4.3` - linux; amd64

```console
$ docker pull vault@sha256:71beaeca153c4cfb27fde00f778468ad5d8d3b6729aca29af5a6f530ac03b7ac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52141093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeff8a0e63ad36dc9b200a6aa38aba61ba3a032d0c0523cb61f68490af4c00cc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 03 Jul 2020 17:20:12 GMT
ARG VAULT_VERSION=1.4.3
# Fri, 03 Jul 2020 17:20:13 GMT
# ARGS: VAULT_VERSION=1.4.3
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 03 Jul 2020 17:20:18 GMT
# ARGS: VAULT_VERSION=1.4.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 03 Jul 2020 17:20:19 GMT
# ARGS: VAULT_VERSION=1.4.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 03 Jul 2020 17:20:19 GMT
VOLUME [/vault/logs]
# Fri, 03 Jul 2020 17:20:19 GMT
VOLUME [/vault/file]
# Fri, 03 Jul 2020 17:20:20 GMT
EXPOSE 8200
# Fri, 03 Jul 2020 17:20:20 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 03 Jul 2020 17:20:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Jul 2020 17:20:20 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33636826a943396873384b2ee6b43c080db2f1920e418b8d2ea33104b5a3efc`  
		Last Modified: Fri, 03 Jul 2020 17:20:40 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38d5932db2a5e4c40690f53207ac6b13b3ac2b3f3ce6b9fdf98e823bc698d15`  
		Last Modified: Fri, 03 Jul 2020 17:20:48 GMT  
		Size: 49.3 MB (49342274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7982fbe652748b20a8efd499c18b93933b2af4ae182e8f1efd3e09b8ce70e3e`  
		Last Modified: Fri, 03 Jul 2020 17:20:40 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5723939fa01f464fa05b331dd1943283486bfa213cb85185fa09271f80854704`  
		Last Modified: Fri, 03 Jul 2020 17:20:40 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.4.3` - linux; arm variant v6

```console
$ docker pull vault@sha256:a7197dee0d6ed411a66def9f0721bbea9c6853084f89a1fa9e59b9f9983205e0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48820703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:225360cf96e2abf2bd5bb1c5efaa0ed7fd4810df1f886e055e991fc206f64d8e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Fri, 03 Jul 2020 16:50:27 GMT
ARG VAULT_VERSION=1.4.3
# Fri, 03 Jul 2020 16:50:30 GMT
# ARGS: VAULT_VERSION=1.4.3
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 03 Jul 2020 16:50:54 GMT
# ARGS: VAULT_VERSION=1.4.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 03 Jul 2020 16:50:56 GMT
# ARGS: VAULT_VERSION=1.4.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 03 Jul 2020 16:50:56 GMT
VOLUME [/vault/logs]
# Fri, 03 Jul 2020 16:50:57 GMT
VOLUME [/vault/file]
# Fri, 03 Jul 2020 16:50:57 GMT
EXPOSE 8200
# Fri, 03 Jul 2020 16:50:58 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 03 Jul 2020 16:50:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Jul 2020 16:50:59 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55fbc041999fc2b59dd451c802e26b955c2c9f45fc376a033644e0fbec7d538`  
		Last Modified: Fri, 03 Jul 2020 16:51:37 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdab99a032b3f65109473b674a16f7ff401d24a23a5364debe26c4696205435`  
		Last Modified: Fri, 03 Jul 2020 16:51:50 GMT  
		Size: 46.2 MB (46244893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2b0cf842ee0b011b893eaadca627380e9af54d97c52a8efb9b6b14f82d64fa`  
		Last Modified: Fri, 03 Jul 2020 16:51:37 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81208e1208a8a16d2e685126cd2040ce76bbdce58676cd885812f35d4fb9ced`  
		Last Modified: Fri, 03 Jul 2020 16:51:37 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.4.3` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:3bbcc754e3bab5b60e1b779958d3d1a27aec7b94fb234f2d974724e2379f7bae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49052848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5046849458e64e9ed99554261ce1d0812cad2de87477389adc94e28177a2a9f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 03 Jul 2020 17:43:45 GMT
ARG VAULT_VERSION=1.4.3
# Fri, 03 Jul 2020 17:43:47 GMT
# ARGS: VAULT_VERSION=1.4.3
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 03 Jul 2020 17:43:55 GMT
# ARGS: VAULT_VERSION=1.4.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 03 Jul 2020 17:43:58 GMT
# ARGS: VAULT_VERSION=1.4.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 03 Jul 2020 17:43:58 GMT
VOLUME [/vault/logs]
# Fri, 03 Jul 2020 17:43:59 GMT
VOLUME [/vault/file]
# Fri, 03 Jul 2020 17:44:00 GMT
EXPOSE 8200
# Fri, 03 Jul 2020 17:44:00 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 03 Jul 2020 17:44:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Jul 2020 17:44:02 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5feb4032d5360f2a4fe8653fda353b146ad66f37b64abe5ed7d0da88c009cf7`  
		Last Modified: Fri, 03 Jul 2020 17:44:33 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87756254c35e80ee04fdd07a4a10b2dc05ba67c163f0e5b906e64ebbcb52f1e`  
		Last Modified: Fri, 03 Jul 2020 17:44:45 GMT  
		Size: 46.3 MB (46330816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659c5fd431bfa4c01d68e8f826f89b942b30c27d65b3653727803a8e3dd334e8`  
		Last Modified: Fri, 03 Jul 2020 17:44:32 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421dd14e7a0b12e75156451fa1aa033b9bf1e61a6f3c566bdbd5476b42032ea7`  
		Last Modified: Fri, 03 Jul 2020 17:44:32 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.4.3` - linux; 386

```console
$ docker pull vault@sha256:7caf492b22bc8582fd6d1dba77b22f1785c89ed81f942cbb63279f38d8ed8ada
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50321413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fff8c2a8230c66903334537ebb3a115c6502ffd2272ff924f8c8979f06919938`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Fri, 03 Jul 2020 17:38:39 GMT
ARG VAULT_VERSION=1.4.3
# Fri, 03 Jul 2020 17:38:40 GMT
# ARGS: VAULT_VERSION=1.4.3
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 03 Jul 2020 17:38:46 GMT
# ARGS: VAULT_VERSION=1.4.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 03 Jul 2020 17:38:46 GMT
# ARGS: VAULT_VERSION=1.4.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 03 Jul 2020 17:38:47 GMT
VOLUME [/vault/logs]
# Fri, 03 Jul 2020 17:38:47 GMT
VOLUME [/vault/file]
# Fri, 03 Jul 2020 17:38:47 GMT
EXPOSE 8200
# Fri, 03 Jul 2020 17:38:47 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 03 Jul 2020 17:38:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Jul 2020 17:38:48 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff13f848775c9d55a090b4c35c7c93750023833d521af2829fcde84219c13e8f`  
		Last Modified: Fri, 03 Jul 2020 17:39:07 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c975e3a53e2c0538c9594f44a147058dc86ab6b60aca3af81d1cf286382deb79`  
		Last Modified: Fri, 03 Jul 2020 17:39:14 GMT  
		Size: 47.5 MB (47531051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb155c6900964d76570ad5e74cffd2846234543be816719e525be2168a8c7dcc`  
		Last Modified: Fri, 03 Jul 2020 17:39:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271e3b37bdae96f4bd21c37ade3be106356aead0a8e2358cfe0ea4c9e779c094`  
		Last Modified: Fri, 03 Jul 2020 17:39:07 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.5.0-rc`

**does not exist** (yet?)

## `vault:latest`

```console
$ docker pull vault@sha256:be3a63905b4d78d6e7c24fc9aacb30621d7a8a1ad8e8baff286a4ba110db16e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:71beaeca153c4cfb27fde00f778468ad5d8d3b6729aca29af5a6f530ac03b7ac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52141093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeff8a0e63ad36dc9b200a6aa38aba61ba3a032d0c0523cb61f68490af4c00cc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 03 Jul 2020 17:20:12 GMT
ARG VAULT_VERSION=1.4.3
# Fri, 03 Jul 2020 17:20:13 GMT
# ARGS: VAULT_VERSION=1.4.3
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 03 Jul 2020 17:20:18 GMT
# ARGS: VAULT_VERSION=1.4.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 03 Jul 2020 17:20:19 GMT
# ARGS: VAULT_VERSION=1.4.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 03 Jul 2020 17:20:19 GMT
VOLUME [/vault/logs]
# Fri, 03 Jul 2020 17:20:19 GMT
VOLUME [/vault/file]
# Fri, 03 Jul 2020 17:20:20 GMT
EXPOSE 8200
# Fri, 03 Jul 2020 17:20:20 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 03 Jul 2020 17:20:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Jul 2020 17:20:20 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33636826a943396873384b2ee6b43c080db2f1920e418b8d2ea33104b5a3efc`  
		Last Modified: Fri, 03 Jul 2020 17:20:40 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38d5932db2a5e4c40690f53207ac6b13b3ac2b3f3ce6b9fdf98e823bc698d15`  
		Last Modified: Fri, 03 Jul 2020 17:20:48 GMT  
		Size: 49.3 MB (49342274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7982fbe652748b20a8efd499c18b93933b2af4ae182e8f1efd3e09b8ce70e3e`  
		Last Modified: Fri, 03 Jul 2020 17:20:40 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5723939fa01f464fa05b331dd1943283486bfa213cb85185fa09271f80854704`  
		Last Modified: Fri, 03 Jul 2020 17:20:40 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:a7197dee0d6ed411a66def9f0721bbea9c6853084f89a1fa9e59b9f9983205e0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48820703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:225360cf96e2abf2bd5bb1c5efaa0ed7fd4810df1f886e055e991fc206f64d8e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Fri, 03 Jul 2020 16:50:27 GMT
ARG VAULT_VERSION=1.4.3
# Fri, 03 Jul 2020 16:50:30 GMT
# ARGS: VAULT_VERSION=1.4.3
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 03 Jul 2020 16:50:54 GMT
# ARGS: VAULT_VERSION=1.4.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 03 Jul 2020 16:50:56 GMT
# ARGS: VAULT_VERSION=1.4.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 03 Jul 2020 16:50:56 GMT
VOLUME [/vault/logs]
# Fri, 03 Jul 2020 16:50:57 GMT
VOLUME [/vault/file]
# Fri, 03 Jul 2020 16:50:57 GMT
EXPOSE 8200
# Fri, 03 Jul 2020 16:50:58 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 03 Jul 2020 16:50:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Jul 2020 16:50:59 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55fbc041999fc2b59dd451c802e26b955c2c9f45fc376a033644e0fbec7d538`  
		Last Modified: Fri, 03 Jul 2020 16:51:37 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdab99a032b3f65109473b674a16f7ff401d24a23a5364debe26c4696205435`  
		Last Modified: Fri, 03 Jul 2020 16:51:50 GMT  
		Size: 46.2 MB (46244893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2b0cf842ee0b011b893eaadca627380e9af54d97c52a8efb9b6b14f82d64fa`  
		Last Modified: Fri, 03 Jul 2020 16:51:37 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81208e1208a8a16d2e685126cd2040ce76bbdce58676cd885812f35d4fb9ced`  
		Last Modified: Fri, 03 Jul 2020 16:51:37 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:3bbcc754e3bab5b60e1b779958d3d1a27aec7b94fb234f2d974724e2379f7bae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49052848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5046849458e64e9ed99554261ce1d0812cad2de87477389adc94e28177a2a9f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 03 Jul 2020 17:43:45 GMT
ARG VAULT_VERSION=1.4.3
# Fri, 03 Jul 2020 17:43:47 GMT
# ARGS: VAULT_VERSION=1.4.3
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 03 Jul 2020 17:43:55 GMT
# ARGS: VAULT_VERSION=1.4.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 03 Jul 2020 17:43:58 GMT
# ARGS: VAULT_VERSION=1.4.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 03 Jul 2020 17:43:58 GMT
VOLUME [/vault/logs]
# Fri, 03 Jul 2020 17:43:59 GMT
VOLUME [/vault/file]
# Fri, 03 Jul 2020 17:44:00 GMT
EXPOSE 8200
# Fri, 03 Jul 2020 17:44:00 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 03 Jul 2020 17:44:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Jul 2020 17:44:02 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5feb4032d5360f2a4fe8653fda353b146ad66f37b64abe5ed7d0da88c009cf7`  
		Last Modified: Fri, 03 Jul 2020 17:44:33 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87756254c35e80ee04fdd07a4a10b2dc05ba67c163f0e5b906e64ebbcb52f1e`  
		Last Modified: Fri, 03 Jul 2020 17:44:45 GMT  
		Size: 46.3 MB (46330816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659c5fd431bfa4c01d68e8f826f89b942b30c27d65b3653727803a8e3dd334e8`  
		Last Modified: Fri, 03 Jul 2020 17:44:32 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421dd14e7a0b12e75156451fa1aa033b9bf1e61a6f3c566bdbd5476b42032ea7`  
		Last Modified: Fri, 03 Jul 2020 17:44:32 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:7caf492b22bc8582fd6d1dba77b22f1785c89ed81f942cbb63279f38d8ed8ada
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50321413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fff8c2a8230c66903334537ebb3a115c6502ffd2272ff924f8c8979f06919938`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Fri, 03 Jul 2020 17:38:39 GMT
ARG VAULT_VERSION=1.4.3
# Fri, 03 Jul 2020 17:38:40 GMT
# ARGS: VAULT_VERSION=1.4.3
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 03 Jul 2020 17:38:46 GMT
# ARGS: VAULT_VERSION=1.4.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 03 Jul 2020 17:38:46 GMT
# ARGS: VAULT_VERSION=1.4.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 03 Jul 2020 17:38:47 GMT
VOLUME [/vault/logs]
# Fri, 03 Jul 2020 17:38:47 GMT
VOLUME [/vault/file]
# Fri, 03 Jul 2020 17:38:47 GMT
EXPOSE 8200
# Fri, 03 Jul 2020 17:38:47 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 03 Jul 2020 17:38:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Jul 2020 17:38:48 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff13f848775c9d55a090b4c35c7c93750023833d521af2829fcde84219c13e8f`  
		Last Modified: Fri, 03 Jul 2020 17:39:07 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c975e3a53e2c0538c9594f44a147058dc86ab6b60aca3af81d1cf286382deb79`  
		Last Modified: Fri, 03 Jul 2020 17:39:14 GMT  
		Size: 47.5 MB (47531051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb155c6900964d76570ad5e74cffd2846234543be816719e525be2168a8c7dcc`  
		Last Modified: Fri, 03 Jul 2020 17:39:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271e3b37bdae96f4bd21c37ade3be106356aead0a8e2358cfe0ea4c9e779c094`  
		Last Modified: Fri, 03 Jul 2020 17:39:07 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
