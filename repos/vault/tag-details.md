<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:1.2.6`](#vault126)
-	[`vault:1.3.9`](#vault139)
-	[`vault:1.4.5`](#vault145)
-	[`vault:1.5.2`](#vault152)
-	[`vault:latest`](#vaultlatest)

## `vault:1.2.6`

```console
$ docker pull vault@sha256:3a66c98a3070eac9cce087aa3ab21e9fb25c51ac799f3ab268ac413f015c0a6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6

### `vault:1.2.6` - linux; arm variant v6

```console
$ docker pull vault@sha256:a27c9d23f4684cae4a96fa8ccefd14a9ef359e18d40a66e7e92ac69649e5f3a5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46537045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31185b73511096c51bbe9177859ea9eeb628b528dbb3f1d9f35c854e2559de0e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Fri, 21 Aug 2020 18:03:48 GMT
ARG VAULT_VERSION=1.2.6
# Fri, 21 Aug 2020 18:04:21 GMT
# ARGS: VAULT_VERSION=1.2.6
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 21 Aug 2020 18:04:59 GMT
# ARGS: VAULT_VERSION=1.2.6
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 21 Aug 2020 18:05:30 GMT
# ARGS: VAULT_VERSION=1.2.6
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 21 Aug 2020 18:05:36 GMT
VOLUME [/vault/logs]
# Fri, 21 Aug 2020 18:05:43 GMT
VOLUME [/vault/file]
# Fri, 21 Aug 2020 18:05:50 GMT
EXPOSE 8200
# Fri, 21 Aug 2020 18:06:03 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 21 Aug 2020 18:06:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Aug 2020 18:06:21 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3710d5164bdf6fb2b649cc62a3ca60b2f7367e7931c4a38c3d1f196cb0b1c5`  
		Last Modified: Fri, 21 Aug 2020 18:07:36 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bfe6db1c60fa2a2c8ca33fbb9be58f021aac53855c0ebe6737050275ea4525`  
		Last Modified: Fri, 21 Aug 2020 18:07:47 GMT  
		Size: 44.0 MB (43961230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74385b379901a95b903e0b50bae9a37fcb89e4e0fe267201a8d9ee0c45989c18`  
		Last Modified: Fri, 21 Aug 2020 18:07:35 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e494efa130628aeaca60b7d885fd0087e0fbfb7b8a6de2939a4885cef01d28`  
		Last Modified: Fri, 21 Aug 2020 18:07:35 GMT  
		Size: 1.8 KB (1826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.3.9`

```console
$ docker pull vault@sha256:68dc464b7a50031884226dc959fe9e42322081fdac916b7322433480fbe53dea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6

### `vault:1.3.9` - linux; arm variant v6

```console
$ docker pull vault@sha256:e5ace478652e361d2515eca96c5fc36019b975fa1a308496ae3cdf1a526d3a6e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48656126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6aa929483b4d069b51b3582331c5322ecf188394ebc513e308ecb19f2374363`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Fri, 21 Aug 2020 18:00:15 GMT
ARG VAULT_VERSION=1.3.9
# Fri, 21 Aug 2020 18:00:52 GMT
# ARGS: VAULT_VERSION=1.3.9
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 21 Aug 2020 18:01:40 GMT
# ARGS: VAULT_VERSION=1.3.9
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 21 Aug 2020 18:02:21 GMT
# ARGS: VAULT_VERSION=1.3.9
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 21 Aug 2020 18:02:30 GMT
VOLUME [/vault/logs]
# Fri, 21 Aug 2020 18:02:36 GMT
VOLUME [/vault/file]
# Fri, 21 Aug 2020 18:02:42 GMT
EXPOSE 8200
# Fri, 21 Aug 2020 18:02:59 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 21 Aug 2020 18:03:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Aug 2020 18:03:22 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6fcb7880a621919f1759cc6eeda5dedde842706a1d0ffb5d5696383c4094853`  
		Last Modified: Fri, 21 Aug 2020 18:07:15 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24bbdc2d2280b70ca9e9ad968f9e0c1167706e09a28482eef19d94651f1ef0ae`  
		Last Modified: Fri, 21 Aug 2020 18:07:28 GMT  
		Size: 46.1 MB (46080313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51bd0d860baebf94bed1d0a9b8890f48c3320ef4a067b3fbad97d3a858fd4bf1`  
		Last Modified: Fri, 21 Aug 2020 18:07:15 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff92b13724d85e931973702bd08bc5ede26b436695ca246d47114bacc3457d8`  
		Last Modified: Fri, 21 Aug 2020 18:07:15 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.4.5`

```console
$ docker pull vault@sha256:d8a37c83d44fb1937b848116df510a08138ecc797d2254331a422c6d67efa003
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6

### `vault:1.4.5` - linux; arm variant v6

```console
$ docker pull vault@sha256:1ea20650a103ad8c9008f01ac0d48d5ba94fc6add3371e91c9765fd323d13f87
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48715199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1d8fb5e33b5b4548c8fdb84d0d5b55d08afc561b2b144c7b6eefdf2c484b816`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Fri, 21 Aug 2020 17:56:49 GMT
ARG VAULT_VERSION=1.4.5
# Fri, 21 Aug 2020 17:57:17 GMT
# ARGS: VAULT_VERSION=1.4.5
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 21 Aug 2020 17:58:03 GMT
# ARGS: VAULT_VERSION=1.4.5
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 21 Aug 2020 17:58:44 GMT
# ARGS: VAULT_VERSION=1.4.5
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 21 Aug 2020 17:58:54 GMT
VOLUME [/vault/logs]
# Fri, 21 Aug 2020 17:59:00 GMT
VOLUME [/vault/file]
# Fri, 21 Aug 2020 17:59:10 GMT
EXPOSE 8200
# Fri, 21 Aug 2020 17:59:27 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 21 Aug 2020 17:59:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Aug 2020 17:59:45 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95b854c6dd2b2f51cbe01e3a4a5cff3eea6351bf4dcd01509f6a136fe94b890`  
		Last Modified: Fri, 21 Aug 2020 18:06:55 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:887a049ac803026f1b467005bb09fd146d9675382594d327bbdb0de755d28971`  
		Last Modified: Fri, 21 Aug 2020 18:07:08 GMT  
		Size: 46.1 MB (46139387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e982690aa4706be10447be1d91bd6844e83d5854d2f7dd4c1a7d344d0b600851`  
		Last Modified: Fri, 21 Aug 2020 18:06:55 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98c320d4b9215d15c6362d43047218a9fbb6804ac0bf62b5317e487dbdeb223`  
		Last Modified: Fri, 21 Aug 2020 18:06:55 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.5.2`

```console
$ docker pull vault@sha256:7f001b218fac531c84fd9fb336f534225e9e0aeb92a83674a5c7c12d3439ad27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6

### `vault:1.5.2` - linux; arm variant v6

```console
$ docker pull vault@sha256:7509003ece487d0ac4df08d5bd7875f4fe97234ec819f91c288056f084c62fa7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51550076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f74a680705453c2fa1ed1e484bd4d7e18f4154efb9c4b531bee5f16b3674c9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Fri, 21 Aug 2020 17:54:15 GMT
ARG VAULT_VERSION=1.5.2
# Fri, 21 Aug 2020 17:54:42 GMT
# ARGS: VAULT_VERSION=1.5.2
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 21 Aug 2020 17:55:21 GMT
# ARGS: VAULT_VERSION=1.5.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 21 Aug 2020 17:55:49 GMT
# ARGS: VAULT_VERSION=1.5.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 21 Aug 2020 17:55:55 GMT
VOLUME [/vault/logs]
# Fri, 21 Aug 2020 17:56:01 GMT
VOLUME [/vault/file]
# Fri, 21 Aug 2020 17:56:07 GMT
EXPOSE 8200
# Fri, 21 Aug 2020 17:56:18 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 21 Aug 2020 17:56:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Aug 2020 17:56:30 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc6abc070bd5f5861e48c418ceac66274d409f1de73c78e209a121bbd1551d7`  
		Last Modified: Fri, 21 Aug 2020 18:06:33 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09dd3f6bdd6fa6c4641034644f1eb16fd2f64e03c9ac9c66e2dbc345d98727a6`  
		Last Modified: Fri, 21 Aug 2020 18:06:46 GMT  
		Size: 49.0 MB (48974263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a023f876d8d7dcbb63a69c0eed38fe28fc8ce32b28ecbfbe51eca4569833071`  
		Last Modified: Fri, 21 Aug 2020 18:06:33 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0ef6bbd727f6920d99b321848bfbddde0c56f4371265a48656fb05c05569e2`  
		Last Modified: Fri, 21 Aug 2020 18:06:33 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:latest`

```console
$ docker pull vault@sha256:e9c163ece5abde2ac1dd544abb8f61435b610bebc536d769196bcc3f5ab3d517
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:93bffce899095d5b085273155515741311bb2dcdd52fb56fbe0f188f71c910fe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.3 MB (54325728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:843dda5d35e1bd42612c15ba3e1f636756596226b93b72f008bfd7dba1a1b86f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Wed, 22 Jul 2020 01:31:55 GMT
ARG VAULT_VERSION=1.5.0
# Wed, 22 Jul 2020 01:31:57 GMT
# ARGS: VAULT_VERSION=1.5.0
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Jul 2020 01:32:06 GMT
# ARGS: VAULT_VERSION=1.5.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Jul 2020 01:32:08 GMT
# ARGS: VAULT_VERSION=1.5.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Jul 2020 01:32:08 GMT
VOLUME [/vault/logs]
# Wed, 22 Jul 2020 01:32:09 GMT
VOLUME [/vault/file]
# Wed, 22 Jul 2020 01:32:09 GMT
EXPOSE 8200
# Wed, 22 Jul 2020 01:32:09 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Jul 2020 01:32:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 01:32:10 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83d0d2835011ad2bfa426f921e713119f9313e412918397a0129ccab01e09c6`  
		Last Modified: Wed, 22 Jul 2020 01:32:19 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b2ebf789aae50091af5d9e17127b37f32f9db0c0a982f57443dbb32e3e704f`  
		Last Modified: Wed, 22 Jul 2020 01:32:32 GMT  
		Size: 51.5 MB (51526910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3cc15a133f4b9ecbcbb30b6f7a73a7816a7b2610f36e52c3eca21d9dc01b8f`  
		Last Modified: Wed, 22 Jul 2020 01:32:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2ee5161fc733a9c81babca2ab2eb74bbfc18569bb4cd025f64d91bf7e831c3`  
		Last Modified: Wed, 22 Jul 2020 01:32:19 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:7509003ece487d0ac4df08d5bd7875f4fe97234ec819f91c288056f084c62fa7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51550076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f74a680705453c2fa1ed1e484bd4d7e18f4154efb9c4b531bee5f16b3674c9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Fri, 21 Aug 2020 17:54:15 GMT
ARG VAULT_VERSION=1.5.2
# Fri, 21 Aug 2020 17:54:42 GMT
# ARGS: VAULT_VERSION=1.5.2
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 21 Aug 2020 17:55:21 GMT
# ARGS: VAULT_VERSION=1.5.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 21 Aug 2020 17:55:49 GMT
# ARGS: VAULT_VERSION=1.5.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 21 Aug 2020 17:55:55 GMT
VOLUME [/vault/logs]
# Fri, 21 Aug 2020 17:56:01 GMT
VOLUME [/vault/file]
# Fri, 21 Aug 2020 17:56:07 GMT
EXPOSE 8200
# Fri, 21 Aug 2020 17:56:18 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 21 Aug 2020 17:56:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Aug 2020 17:56:30 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc6abc070bd5f5861e48c418ceac66274d409f1de73c78e209a121bbd1551d7`  
		Last Modified: Fri, 21 Aug 2020 18:06:33 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09dd3f6bdd6fa6c4641034644f1eb16fd2f64e03c9ac9c66e2dbc345d98727a6`  
		Last Modified: Fri, 21 Aug 2020 18:06:46 GMT  
		Size: 49.0 MB (48974263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a023f876d8d7dcbb63a69c0eed38fe28fc8ce32b28ecbfbe51eca4569833071`  
		Last Modified: Fri, 21 Aug 2020 18:06:33 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0ef6bbd727f6920d99b321848bfbddde0c56f4371265a48656fb05c05569e2`  
		Last Modified: Fri, 21 Aug 2020 18:06:33 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:ff596cf9df78a300904af5808996eba930c8af17e2877536e88e723bfdbdc78c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51261501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bc4ed95de203cae2ffac8294a9c0aaf470fd5f430e60f0a614c15d2448fc047`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Wed, 22 Jul 2020 00:53:11 GMT
ARG VAULT_VERSION=1.5.0
# Wed, 22 Jul 2020 00:53:15 GMT
# ARGS: VAULT_VERSION=1.5.0
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Jul 2020 00:53:23 GMT
# ARGS: VAULT_VERSION=1.5.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Jul 2020 00:53:27 GMT
# ARGS: VAULT_VERSION=1.5.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Jul 2020 00:53:28 GMT
VOLUME [/vault/logs]
# Wed, 22 Jul 2020 00:53:28 GMT
VOLUME [/vault/file]
# Wed, 22 Jul 2020 00:53:29 GMT
EXPOSE 8200
# Wed, 22 Jul 2020 00:53:30 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Jul 2020 00:53:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 00:53:31 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34f3c292160241915a90468ebd833263004f79dc31f19c6b55022c5bc23f425`  
		Last Modified: Wed, 22 Jul 2020 00:53:41 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969828cd481f598b339f4f94d09524a2385c07cf4cd41fdc64e76dbd30fd8b91`  
		Last Modified: Wed, 22 Jul 2020 00:53:53 GMT  
		Size: 48.5 MB (48539468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89bc576029a71c33adcb793b8ce72231f54246ca41bb41dc81ce149ff7212e7`  
		Last Modified: Wed, 22 Jul 2020 00:53:41 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73d93c42445059eaf0931ec83de1981371fd2a665384e43b8d58f5f5471e1a3`  
		Last Modified: Wed, 22 Jul 2020 00:53:41 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:73e6d355c750f7ea852533734fead354d69c2526639e5978ac55e25e1f02a6d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52448518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02d5d0f6b760ba955d94c40e784ac2f01a3657755c0b61371571b0c53a2cf0ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Wed, 22 Jul 2020 02:20:52 GMT
ARG VAULT_VERSION=1.5.0
# Wed, 22 Jul 2020 02:20:53 GMT
# ARGS: VAULT_VERSION=1.5.0
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Jul 2020 02:21:00 GMT
# ARGS: VAULT_VERSION=1.5.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Jul 2020 02:21:00 GMT
# ARGS: VAULT_VERSION=1.5.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Jul 2020 02:21:01 GMT
VOLUME [/vault/logs]
# Wed, 22 Jul 2020 02:21:01 GMT
VOLUME [/vault/file]
# Wed, 22 Jul 2020 02:21:01 GMT
EXPOSE 8200
# Wed, 22 Jul 2020 02:21:01 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Jul 2020 02:21:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 02:21:02 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa6a4c14afcfefd047fd4c94647e87826f05c4a990e16fb2d7ba7b7bf1af2b5`  
		Last Modified: Wed, 22 Jul 2020 02:21:09 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3c4d290c2c65c69f7eae170d528203af72fc61e444f563b797f1907a556bcc`  
		Last Modified: Wed, 22 Jul 2020 02:21:18 GMT  
		Size: 49.7 MB (49658153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264fe782cf6cf4084484d38b675307e796bfaea00d8a3a66575500a82e586dbe`  
		Last Modified: Wed, 22 Jul 2020 02:21:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f27b55f8608662f53633b5036672f840dd1615868ada5247152bbff82f1cfe`  
		Last Modified: Wed, 22 Jul 2020 02:21:09 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
