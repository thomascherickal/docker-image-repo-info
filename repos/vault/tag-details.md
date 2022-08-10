<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:1.10.5`](#vault1105)
-	[`vault:1.11.2`](#vault1112)
-	[`vault:1.8.12`](#vault1812)
-	[`vault:1.9.8`](#vault198)
-	[`vault:latest`](#vaultlatest)

## `vault:1.10.5`

```console
$ docker pull vault@sha256:8498b9f6123530aa63e2c5d3d82528cfb5ebe8297c163051f5b44d13cc24ec8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.10.5` - linux; amd64

```console
$ docker pull vault@sha256:248e4c3289f8a283ba667946ff4fcc4136fccefc69795e0dd93551db4fd2c80f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74112593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6e9378f5a9aadee618030e660496d22e9b01299428e757e1d610000f7682c3d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:27:05 GMT
ARG VAULT_VERSION=1.10.5
# Wed, 10 Aug 2022 01:27:06 GMT
# ARGS: VAULT_VERSION=1.10.5
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 10 Aug 2022 01:27:14 GMT
# ARGS: VAULT_VERSION=1.10.5
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 10 Aug 2022 01:27:15 GMT
# ARGS: VAULT_VERSION=1.10.5
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 10 Aug 2022 01:27:15 GMT
VOLUME [/vault/logs]
# Wed, 10 Aug 2022 01:27:15 GMT
VOLUME [/vault/file]
# Wed, 10 Aug 2022 01:27:15 GMT
EXPOSE 8200
# Wed, 10 Aug 2022 01:27:15 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 10 Aug 2022 01:27:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 01:27:15 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d2e8f0e60b2388a148048bc944a645c34b00b362868f8ee4ebc2202e5e0be7`  
		Last Modified: Wed, 10 Aug 2022 01:28:10 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61f82dfb57a76942d8208187861dc2be244472c48188a4a153f8d8c7034dab0`  
		Last Modified: Wed, 10 Aug 2022 01:28:19 GMT  
		Size: 71.3 MB (71281838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0eb465fdfc83330a84257c80e1c6f3ba709697f7f6dd1468753e73424ecff7b`  
		Last Modified: Wed, 10 Aug 2022 01:28:10 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1512ca7d764e4b8e92497a47ed1a8f2f4a4104e6cc66dfc4af99258f43c17a4d`  
		Last Modified: Wed, 10 Aug 2022 01:28:10 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.10.5` - linux; arm variant v6

```console
$ docker pull vault@sha256:d2764da758ee0ef730d2049a132bd815e5393992d79cc65c212c3659a8ccea39
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67370801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b52036f5db7c3fc3245670bebcf9c034a6a94781f54f0ef1027da0c5129823f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:50:02 GMT
ADD file:5a22b2130f6fbe534730df1f47715641a45e55845be7f35c3183e2b74ec43397 in / 
# Tue, 19 Jul 2022 22:50:03 GMT
CMD ["/bin/sh"]
# Thu, 04 Aug 2022 00:50:10 GMT
ARG VAULT_VERSION=1.10.5
# Thu, 04 Aug 2022 00:50:11 GMT
# ARGS: VAULT_VERSION=1.10.5
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 04 Aug 2022 00:50:21 GMT
# ARGS: VAULT_VERSION=1.10.5
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 04 Aug 2022 00:50:22 GMT
# ARGS: VAULT_VERSION=1.10.5
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 04 Aug 2022 00:50:22 GMT
VOLUME [/vault/logs]
# Thu, 04 Aug 2022 00:50:22 GMT
VOLUME [/vault/file]
# Thu, 04 Aug 2022 00:50:23 GMT
EXPOSE 8200
# Thu, 04 Aug 2022 00:50:23 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 04 Aug 2022 00:50:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 00:50:23 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:7dc1cbfb63ac7071e143ce96f0f140dc30282039f8d0770eaa7ab97eba515639`  
		Last Modified: Tue, 19 Jul 2022 22:51:41 GMT  
		Size: 2.6 MB (2626632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532eccdb436743b150d04bd3f946df16ef2f0a70838a2374863f0baa66615274`  
		Last Modified: Thu, 04 Aug 2022 00:51:50 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7ed19dc0844bb5b2a977bbd6204437c9d7542ce636d05df034228d424f2934`  
		Last Modified: Thu, 04 Aug 2022 00:52:03 GMT  
		Size: 64.7 MB (64740899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f50c5f7a5c7e982e92340d4cf02a6b866a358421baaf7b9b37d61ba9efeb3ca`  
		Last Modified: Thu, 04 Aug 2022 00:51:50 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c4a89cbcbc8e6a03abcdded7f408f609b572230ef0e0da31d456969173e0c6`  
		Last Modified: Thu, 04 Aug 2022 00:51:50 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.10.5` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:4ecb1ffa3f685473eaa5a782e898dc315cd885179570dad5228e0db93a0e22c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69132755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4418711d73c85745d314136bbb0a731a206a56ce5edfdf5b8573df80b6a2f4dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:39:51 GMT
ADD file:bb30934245445dabbe698387b5d454c2360d05055f7ab1bcaaffefea5aefb539 in / 
# Tue, 19 Jul 2022 22:39:51 GMT
CMD ["/bin/sh"]
# Mon, 25 Jul 2022 18:47:19 GMT
ARG VAULT_VERSION=1.10.5
# Mon, 25 Jul 2022 18:47:20 GMT
# ARGS: VAULT_VERSION=1.10.5
RUN addgroup vault &&     adduser -S -G vault vault
# Mon, 25 Jul 2022 18:47:27 GMT
# ARGS: VAULT_VERSION=1.10.5
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Mon, 25 Jul 2022 18:47:27 GMT
# ARGS: VAULT_VERSION=1.10.5
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Mon, 25 Jul 2022 18:47:28 GMT
VOLUME [/vault/logs]
# Mon, 25 Jul 2022 18:47:29 GMT
VOLUME [/vault/file]
# Mon, 25 Jul 2022 18:47:30 GMT
EXPOSE 8200
# Mon, 25 Jul 2022 18:47:32 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jul 2022 18:47:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jul 2022 18:47:33 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:f4bf3852c6ccaad2dedd57347d310f084247a2e202c2fc20f5fa88d921e8510e`  
		Last Modified: Tue, 19 Jul 2022 22:40:44 GMT  
		Size: 2.7 MB (2717747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3f17a8ac6bc03dd8068241227da9a24f5326bdccc96be920b779641bc3c4d1`  
		Last Modified: Mon, 25 Jul 2022 18:48:36 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cbac59670e650333995fb367b7687f003d19498aff5532a5b61808bcdededf`  
		Last Modified: Mon, 25 Jul 2022 18:48:45 GMT  
		Size: 66.4 MB (66411797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6988409cc9551f18a05b17c72b7ead8d0104116934faf7fa0c8a0a8c4f6c954a`  
		Last Modified: Mon, 25 Jul 2022 18:48:36 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3057349c20837d5d7db797adf80aca4ef441d382abe2a0f84e7e678deb1d24e8`  
		Last Modified: Mon, 25 Jul 2022 18:48:36 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.10.5` - linux; 386

```console
$ docker pull vault@sha256:e8852c2e06945042c9b6c36c907e5eb9f86823fc4283cbf38ba00cb42ca10089
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.5 MB (70456174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b9655b3425ef5eb8ea5af8decfe73de443d9c5dcb586a86694f46cbe3478b38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:54 GMT
ADD file:fea8a3ba06779852956b0d3a2dd7514ab33217b1fd395231864c443797f077f6 in / 
# Tue, 09 Aug 2022 17:38:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 00:14:01 GMT
ARG VAULT_VERSION=1.10.5
# Wed, 10 Aug 2022 00:14:02 GMT
# ARGS: VAULT_VERSION=1.10.5
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 10 Aug 2022 00:14:11 GMT
# ARGS: VAULT_VERSION=1.10.5
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 10 Aug 2022 00:14:11 GMT
# ARGS: VAULT_VERSION=1.10.5
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 10 Aug 2022 00:14:12 GMT
VOLUME [/vault/logs]
# Wed, 10 Aug 2022 00:14:13 GMT
VOLUME [/vault/file]
# Wed, 10 Aug 2022 00:14:14 GMT
EXPOSE 8200
# Wed, 10 Aug 2022 00:14:16 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 10 Aug 2022 00:14:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 00:14:17 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:2c44f983a875883421e7d5bc471f6437e0e377e6e7343b52c856caee71064d31`  
		Last Modified: Tue, 09 Aug 2022 17:40:01 GMT  
		Size: 2.8 MB (2832612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fc7ca3ffe898e856f209104e70057a35365e1c6a12edecd6b87954e4b75d84`  
		Last Modified: Wed, 10 Aug 2022 00:15:47 GMT  
		Size: 1.2 KB (1237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30dc3d0657854b104dd9a2cdebdd7d90b7ebd4efa10c9f3d00a9485a669f78f7`  
		Last Modified: Wed, 10 Aug 2022 00:16:00 GMT  
		Size: 67.6 MB (67620361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992a3af5417dfeebd9dd19dc0b3bec31620614d8d63ea6f80028936d0c241db3`  
		Last Modified: Wed, 10 Aug 2022 00:15:47 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ba4a7f20b0f9d667e36f50aed2a06c245706c8be62d39cc13266c8e7bcbc48`  
		Last Modified: Wed, 10 Aug 2022 00:15:47 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.11.2`

```console
$ docker pull vault@sha256:9aa645f2ae2963d803dbb7524679950f451fa4456865ff6454d2a8e0adac5e48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.11.2` - linux; amd64

```console
$ docker pull vault@sha256:7a238778738551ab26e07ef2c4ac9d9d9e8d393ec9e766301c9b3bb0fa5f2b55
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.5 MB (77492763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22fdc6314051df714eb280680c24524ed01d0ed2eddff1358cc40d528c82579e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:26:51 GMT
ARG VAULT_VERSION=1.11.2
# Wed, 10 Aug 2022 01:26:52 GMT
# ARGS: VAULT_VERSION=1.11.2
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 10 Aug 2022 01:27:00 GMT
# ARGS: VAULT_VERSION=1.11.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 10 Aug 2022 01:27:01 GMT
# ARGS: VAULT_VERSION=1.11.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 10 Aug 2022 01:27:01 GMT
VOLUME [/vault/logs]
# Wed, 10 Aug 2022 01:27:01 GMT
VOLUME [/vault/file]
# Wed, 10 Aug 2022 01:27:01 GMT
EXPOSE 8200
# Wed, 10 Aug 2022 01:27:01 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 10 Aug 2022 01:27:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 01:27:01 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8967aa5130c8a6f6bb7143c8391df393368db6921ab770555efde013985a9d28`  
		Last Modified: Wed, 10 Aug 2022 01:27:51 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db9d0afc6ab490c62cd716176a04cfd75c36714cb67b9e30a2cda0ef0be75f0`  
		Last Modified: Wed, 10 Aug 2022 01:28:01 GMT  
		Size: 74.7 MB (74662006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0119f940dd249e511bdcf111cbe3b317d64b16eaa192d25fb6b9d83326f33acb`  
		Last Modified: Wed, 10 Aug 2022 01:27:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98184bebb2e9dc29170e6960d8239418e57b92f48ef4edd5a62482071df9c373`  
		Last Modified: Wed, 10 Aug 2022 01:27:51 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.11.2` - linux; arm variant v6

```console
$ docker pull vault@sha256:f7b36d61ef1e198262a672601f06e50c01800f197876613fe38eeaaf19e6faf8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70252099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4840ff699b78218305dbfaa6f8a4e5e4fd09a28544ecfc18f38ee02b39a7bcdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:50:02 GMT
ADD file:5a22b2130f6fbe534730df1f47715641a45e55845be7f35c3183e2b74ec43397 in / 
# Tue, 19 Jul 2022 22:50:03 GMT
CMD ["/bin/sh"]
# Thu, 04 Aug 2022 00:49:49 GMT
ARG VAULT_VERSION=1.11.2
# Thu, 04 Aug 2022 00:49:50 GMT
# ARGS: VAULT_VERSION=1.11.2
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 04 Aug 2022 00:50:03 GMT
# ARGS: VAULT_VERSION=1.11.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 04 Aug 2022 00:50:04 GMT
# ARGS: VAULT_VERSION=1.11.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 04 Aug 2022 00:50:04 GMT
VOLUME [/vault/logs]
# Thu, 04 Aug 2022 00:50:04 GMT
VOLUME [/vault/file]
# Thu, 04 Aug 2022 00:50:04 GMT
EXPOSE 8200
# Thu, 04 Aug 2022 00:50:05 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 04 Aug 2022 00:50:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 00:50:05 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:7dc1cbfb63ac7071e143ce96f0f140dc30282039f8d0770eaa7ab97eba515639`  
		Last Modified: Tue, 19 Jul 2022 22:51:41 GMT  
		Size: 2.6 MB (2626632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe5d0bab33752d600ccc29fbfe614ed9b77022cc6917e0d105f43029315d5c1`  
		Last Modified: Thu, 04 Aug 2022 00:51:25 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddad393ff0b354750574a05b6092fc9d6af3767312789455a8e557815014dca`  
		Last Modified: Thu, 04 Aug 2022 00:51:38 GMT  
		Size: 67.6 MB (67622196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4fd1bd01fd74ec5a209c0e8ef421017bbc7c6710c69b8167bb4973fbd35d84`  
		Last Modified: Thu, 04 Aug 2022 00:51:25 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8aa266ce16913028810350646722976666d954374379b285b0f65ba4337da8`  
		Last Modified: Thu, 04 Aug 2022 00:51:25 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.11.2` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:a5e9ea80e35ff247cf83cc7ab06022c50366d7e36ec1135e4d740b7496bb201e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72280976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74e752c8d20377f9028c78a12d70d10ac833656174e6e64c9df558a3e5a0655d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:39:51 GMT
ADD file:bb30934245445dabbe698387b5d454c2360d05055f7ab1bcaaffefea5aefb539 in / 
# Tue, 19 Jul 2022 22:39:51 GMT
CMD ["/bin/sh"]
# Thu, 04 Aug 2022 00:42:15 GMT
ARG VAULT_VERSION=1.11.2
# Thu, 04 Aug 2022 00:42:16 GMT
# ARGS: VAULT_VERSION=1.11.2
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 04 Aug 2022 00:42:25 GMT
# ARGS: VAULT_VERSION=1.11.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 04 Aug 2022 00:42:26 GMT
# ARGS: VAULT_VERSION=1.11.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 04 Aug 2022 00:42:26 GMT
VOLUME [/vault/logs]
# Thu, 04 Aug 2022 00:42:27 GMT
VOLUME [/vault/file]
# Thu, 04 Aug 2022 00:42:28 GMT
EXPOSE 8200
# Thu, 04 Aug 2022 00:42:30 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 04 Aug 2022 00:42:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 00:42:31 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:f4bf3852c6ccaad2dedd57347d310f084247a2e202c2fc20f5fa88d921e8510e`  
		Last Modified: Tue, 19 Jul 2022 22:40:44 GMT  
		Size: 2.7 MB (2717747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b09458246504b8537fdc40489d178a1162f42ae33f83d1668f22dbbb02618d`  
		Last Modified: Thu, 04 Aug 2022 00:43:02 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f72f8bcd3c8ec0587c1e140832995309ee204e3156ecf582e9837f3eb65f64`  
		Last Modified: Thu, 04 Aug 2022 00:43:10 GMT  
		Size: 69.6 MB (69560017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0db6c642a591863aed2683b2e9bc4e30ceb7f6d2a809fe973dc200c155bfd8d`  
		Last Modified: Thu, 04 Aug 2022 00:43:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493a5d945bb81c3d49c8e11b278e072bc4f9df393039f72357a332239acf4672`  
		Last Modified: Thu, 04 Aug 2022 00:43:02 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.11.2` - linux; 386

```console
$ docker pull vault@sha256:556137692bc84155dc5886a12ae852d4ce1d5bb058e207d43a07f5ce716f0808
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73567722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9c7a4e16b968a99b1ef223d5cde6b79ad51103581802e72741be70c9ea5db3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:54 GMT
ADD file:fea8a3ba06779852956b0d3a2dd7514ab33217b1fd395231864c443797f077f6 in / 
# Tue, 09 Aug 2022 17:38:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 00:13:39 GMT
ARG VAULT_VERSION=1.11.2
# Wed, 10 Aug 2022 00:13:40 GMT
# ARGS: VAULT_VERSION=1.11.2
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 10 Aug 2022 00:13:49 GMT
# ARGS: VAULT_VERSION=1.11.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 10 Aug 2022 00:13:50 GMT
# ARGS: VAULT_VERSION=1.11.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 10 Aug 2022 00:13:51 GMT
VOLUME [/vault/logs]
# Wed, 10 Aug 2022 00:13:52 GMT
VOLUME [/vault/file]
# Wed, 10 Aug 2022 00:13:53 GMT
EXPOSE 8200
# Wed, 10 Aug 2022 00:13:55 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 10 Aug 2022 00:13:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 00:13:56 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:2c44f983a875883421e7d5bc471f6437e0e377e6e7343b52c856caee71064d31`  
		Last Modified: Tue, 09 Aug 2022 17:40:01 GMT  
		Size: 2.8 MB (2832612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fdb4858833cdfc5a5714d5a19c93b337a0e778ec7d80ef77189fac0471c7566`  
		Last Modified: Wed, 10 Aug 2022 00:15:25 GMT  
		Size: 1.2 KB (1237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb24cb72e1a2fdb06de8d1a5f75cd0a549f107b77909b2a0c1b20f9e2d74d29`  
		Last Modified: Wed, 10 Aug 2022 00:15:36 GMT  
		Size: 70.7 MB (70731906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7744188d2a7166aef058bb6d424153beba212e4c8749f465cf86914a226ca7`  
		Last Modified: Wed, 10 Aug 2022 00:15:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90460ac0bbb803713f9962bf787cb7021494e0163af9926e3ac5956d65c240d`  
		Last Modified: Wed, 10 Aug 2022 00:15:25 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.8.12`

```console
$ docker pull vault@sha256:9704c634d40311d6239162321b9c7b7b93575d5229e39a1115af12f598bfd5f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.8.12` - linux; amd64

```console
$ docker pull vault@sha256:68f1682b1398535f86c3ecc09c9cde329520b4a67b801da5fa16c92d02641805
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70650989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df9d919fd4756f45ab5c06c05a9eaf2a30867eb5879d2f0859938450515a50f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:27:31 GMT
ARG VAULT_VERSION=1.8.12
# Wed, 10 Aug 2022 01:27:31 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 10 Aug 2022 01:27:39 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 10 Aug 2022 01:27:40 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 10 Aug 2022 01:27:40 GMT
VOLUME [/vault/logs]
# Wed, 10 Aug 2022 01:27:40 GMT
VOLUME [/vault/file]
# Wed, 10 Aug 2022 01:27:40 GMT
EXPOSE 8200
# Wed, 10 Aug 2022 01:27:40 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 10 Aug 2022 01:27:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 01:27:40 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c699ea2f983cbe4bbb320b0b24d2ca4e1f5dab55991affbd9d716508728ce3`  
		Last Modified: Wed, 10 Aug 2022 01:28:41 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589d0c73806458dde55a3c4388d26f54502d3f4e5abf10249a9e06737e51e54e`  
		Last Modified: Wed, 10 Aug 2022 01:28:51 GMT  
		Size: 67.8 MB (67820233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5594347fcf83dd3374582fc6cb35e5570af2304daae67aabc85736eb5ea4c1`  
		Last Modified: Wed, 10 Aug 2022 01:28:42 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957abd22bbfede163b1d7a2bf3fd8d4b02b7a3704e8effd5420d54bad2f97e65`  
		Last Modified: Wed, 10 Aug 2022 01:28:41 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.8.12` - linux; arm variant v6

```console
$ docker pull vault@sha256:9aea82e4242c7fe0b0f0ee04723a3d6b69989fcd305b280ef6377d82d1eb9013
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (64970541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e2bbf706bdcb76eefb04cc3cc0f66a55bd82185d6ad63ff51516c30232fafdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:50:02 GMT
ADD file:5a22b2130f6fbe534730df1f47715641a45e55845be7f35c3183e2b74ec43397 in / 
# Tue, 19 Jul 2022 22:50:03 GMT
CMD ["/bin/sh"]
# Thu, 04 Aug 2022 00:50:50 GMT
ARG VAULT_VERSION=1.8.12
# Thu, 04 Aug 2022 00:50:50 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 04 Aug 2022 00:51:00 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 04 Aug 2022 00:51:01 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 04 Aug 2022 00:51:01 GMT
VOLUME [/vault/logs]
# Thu, 04 Aug 2022 00:51:01 GMT
VOLUME [/vault/file]
# Thu, 04 Aug 2022 00:51:02 GMT
EXPOSE 8200
# Thu, 04 Aug 2022 00:51:02 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 04 Aug 2022 00:51:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 00:51:02 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:7dc1cbfb63ac7071e143ce96f0f140dc30282039f8d0770eaa7ab97eba515639`  
		Last Modified: Tue, 19 Jul 2022 22:51:41 GMT  
		Size: 2.6 MB (2626632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9573a1f0086f0ee0c0084766c143803113dfd2e308ccbe9986ab1b11c2aaa193`  
		Last Modified: Thu, 04 Aug 2022 00:52:33 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42bbeb3379a562d968d1fa06621295d2946c8ff02b6150a309a89f7ed1e58fd7`  
		Last Modified: Thu, 04 Aug 2022 00:52:45 GMT  
		Size: 62.3 MB (62340641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a868d9cf8390f29dd5d0cdac362bafff8976331d8e30f019cced5a73777dcaa`  
		Last Modified: Thu, 04 Aug 2022 00:52:33 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20790f3519dc8db33ba1b6a90aa5b0738cb330b2e55debdd77fab72b22c28407`  
		Last Modified: Thu, 04 Aug 2022 00:52:33 GMT  
		Size: 1.8 KB (1810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.8.12` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:949fab7fb7e5e74dd7ba87f0d9b8d6f582d7ecbfa63550cf2dcc72684ce06365
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66894495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c33ec0af9ce73fce03331993cb0a4b29442d77cd215865d7b701fd11ddfb3ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:39:51 GMT
ADD file:bb30934245445dabbe698387b5d454c2360d05055f7ab1bcaaffefea5aefb539 in / 
# Tue, 19 Jul 2022 22:39:51 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 03:51:38 GMT
ARG VAULT_VERSION=1.8.12
# Wed, 20 Jul 2022 03:51:39 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 20 Jul 2022 03:51:46 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 20 Jul 2022 03:51:47 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 20 Jul 2022 03:51:48 GMT
VOLUME [/vault/logs]
# Wed, 20 Jul 2022 03:51:49 GMT
VOLUME [/vault/file]
# Wed, 20 Jul 2022 03:51:50 GMT
EXPOSE 8200
# Wed, 20 Jul 2022 03:51:52 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 20 Jul 2022 03:51:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 03:51:53 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:f4bf3852c6ccaad2dedd57347d310f084247a2e202c2fc20f5fa88d921e8510e`  
		Last Modified: Tue, 19 Jul 2022 22:40:44 GMT  
		Size: 2.7 MB (2717747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5739e7300a3f66f5f739195564c911c9993c36c3b4f324135a61c92283e68d`  
		Last Modified: Wed, 20 Jul 2022 03:53:04 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292ee0d66eeb81c4100ff44e627e07789f0ceb8957d5973a8972b27afc4ed85b`  
		Last Modified: Wed, 20 Jul 2022 03:53:13 GMT  
		Size: 64.2 MB (64173545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b075f1388274672299fa3c442ac428883b29b402787c9787d6c6937966b1887`  
		Last Modified: Wed, 20 Jul 2022 03:53:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09037a42f58c1807755b846e6c1709cd3ab8a9cda3938d1c081b4d7c8ab8c01c`  
		Last Modified: Wed, 20 Jul 2022 03:53:05 GMT  
		Size: 1.8 KB (1810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.8.12` - linux; 386

```console
$ docker pull vault@sha256:770e659d0eec23e23f4a01203b7b9bb6665cc7c2893d2e678743742f4101a5f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68350476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:706ae3042de1317568c9d824ac6096cbe0af6f93becc8ff08f4b5672c4c87599`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:54 GMT
ADD file:fea8a3ba06779852956b0d3a2dd7514ab33217b1fd395231864c443797f077f6 in / 
# Tue, 09 Aug 2022 17:38:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 00:14:46 GMT
ARG VAULT_VERSION=1.8.12
# Wed, 10 Aug 2022 00:14:47 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 10 Aug 2022 00:14:57 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 10 Aug 2022 00:14:57 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 10 Aug 2022 00:14:58 GMT
VOLUME [/vault/logs]
# Wed, 10 Aug 2022 00:14:59 GMT
VOLUME [/vault/file]
# Wed, 10 Aug 2022 00:15:00 GMT
EXPOSE 8200
# Wed, 10 Aug 2022 00:15:02 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 10 Aug 2022 00:15:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 00:15:03 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:2c44f983a875883421e7d5bc471f6437e0e377e6e7343b52c856caee71064d31`  
		Last Modified: Tue, 09 Aug 2022 17:40:01 GMT  
		Size: 2.8 MB (2832612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d5d18c74e1fbdfe601565cc2bc0d42ac70a255339ed77f0a129d71fef15c5c`  
		Last Modified: Wed, 10 Aug 2022 00:16:30 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c502c38af5250b35fe68bc131779469e8da9589b6a054257fcc0a56787b918`  
		Last Modified: Wed, 10 Aug 2022 00:16:37 GMT  
		Size: 65.5 MB (65514657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c00963d2baa2486178f1d1d0cf2685e4b381f62bc3616e7ea48b1584c81787`  
		Last Modified: Wed, 10 Aug 2022 00:16:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68592ac5ae287cfe31dac3a2bb3bebbbb2088143f4200e61330c5d6635d63aca`  
		Last Modified: Wed, 10 Aug 2022 00:16:30 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.9.8`

```console
$ docker pull vault@sha256:eb811a6eda8f8d09f37d5a8f60537e5dd5aac30d43467f309cc35b96e3cebdca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.9.8` - linux; amd64

```console
$ docker pull vault@sha256:77968904603ab968c31d94f1c359499d0dccb85fb98d813283b7c94cfba9d5b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73221384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eb66e725580e92965befb94623034320b392c3520007285222dd264ed76294f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:27:19 GMT
ARG VAULT_VERSION=1.9.8
# Wed, 10 Aug 2022 01:27:20 GMT
# ARGS: VAULT_VERSION=1.9.8
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 10 Aug 2022 01:27:27 GMT
# ARGS: VAULT_VERSION=1.9.8
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 10 Aug 2022 01:27:28 GMT
# ARGS: VAULT_VERSION=1.9.8
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 10 Aug 2022 01:27:28 GMT
VOLUME [/vault/logs]
# Wed, 10 Aug 2022 01:27:28 GMT
VOLUME [/vault/file]
# Wed, 10 Aug 2022 01:27:28 GMT
EXPOSE 8200
# Wed, 10 Aug 2022 01:27:28 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 10 Aug 2022 01:27:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 01:27:29 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec513384d58fd9d79f418630bd4dd19ade1826e4157fbd88f669099104459e4`  
		Last Modified: Wed, 10 Aug 2022 01:28:25 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6432401cead10728f899d95a1f0beeb2a1d3f2af59a7bdeee4aa810ee03f6f52`  
		Last Modified: Wed, 10 Aug 2022 01:28:34 GMT  
		Size: 70.4 MB (70390629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43f9c9bb1e295ea5ea934060d8a7562de968793dc68a28de60350c00c091075`  
		Last Modified: Wed, 10 Aug 2022 01:28:25 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1b2538e9cc1272c9c2a2a216cb5ec347eb1f8c50498b23d0324c37ecf03fe4`  
		Last Modified: Wed, 10 Aug 2022 01:28:26 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.9.8` - linux; arm variant v6

```console
$ docker pull vault@sha256:00fadaaf551a29b81685a13fadd4d854de472084c335bd794825028aa22bf66d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66532247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a550737fa8d8813ed71fc2d72263c6a40ee30c52ec43f4db88624a3c665060d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:50:02 GMT
ADD file:5a22b2130f6fbe534730df1f47715641a45e55845be7f35c3183e2b74ec43397 in / 
# Tue, 19 Jul 2022 22:50:03 GMT
CMD ["/bin/sh"]
# Thu, 04 Aug 2022 00:50:28 GMT
ARG VAULT_VERSION=1.9.8
# Thu, 04 Aug 2022 00:50:29 GMT
# ARGS: VAULT_VERSION=1.9.8
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 04 Aug 2022 00:50:42 GMT
# ARGS: VAULT_VERSION=1.9.8
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 04 Aug 2022 00:50:43 GMT
# ARGS: VAULT_VERSION=1.9.8
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 04 Aug 2022 00:50:43 GMT
VOLUME [/vault/logs]
# Thu, 04 Aug 2022 00:50:43 GMT
VOLUME [/vault/file]
# Thu, 04 Aug 2022 00:50:43 GMT
EXPOSE 8200
# Thu, 04 Aug 2022 00:50:43 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 04 Aug 2022 00:50:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 00:50:44 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:7dc1cbfb63ac7071e143ce96f0f140dc30282039f8d0770eaa7ab97eba515639`  
		Last Modified: Tue, 19 Jul 2022 22:51:41 GMT  
		Size: 2.6 MB (2626632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b85abe06c417433795f0e0aca4e4793e181c025fd1e2fe8366f2e0c97b94cd`  
		Last Modified: Thu, 04 Aug 2022 00:52:11 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8182267e0f9bf9393f6fa38859bef037c2f464308cc5e27955e6837d402b2`  
		Last Modified: Thu, 04 Aug 2022 00:52:24 GMT  
		Size: 63.9 MB (63902342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace1a9f57b99d3d6340b982674b7fdb9ebbd3a0cbf177c40c6e2982d70016b13`  
		Last Modified: Thu, 04 Aug 2022 00:52:12 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72524e63d417c6c7dc40d46957b790eafa1a947834a9b4f4eec9f7fca9bff72`  
		Last Modified: Thu, 04 Aug 2022 00:52:11 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.9.8` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:adbdebeedb5dd1b435af34f4f0560ec36c1daaeafa02abbe80e9352f28515e87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68298600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f8ffe037f74d5474787e312d476a9ce091e6c4428df18383ec521295f43e028`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:39:51 GMT
ADD file:bb30934245445dabbe698387b5d454c2360d05055f7ab1bcaaffefea5aefb539 in / 
# Tue, 19 Jul 2022 22:39:51 GMT
CMD ["/bin/sh"]
# Mon, 25 Jul 2022 18:47:38 GMT
ARG VAULT_VERSION=1.9.8
# Mon, 25 Jul 2022 18:47:39 GMT
# ARGS: VAULT_VERSION=1.9.8
RUN addgroup vault &&     adduser -S -G vault vault
# Mon, 25 Jul 2022 18:47:47 GMT
# ARGS: VAULT_VERSION=1.9.8
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Mon, 25 Jul 2022 18:47:47 GMT
# ARGS: VAULT_VERSION=1.9.8
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Mon, 25 Jul 2022 18:47:48 GMT
VOLUME [/vault/logs]
# Mon, 25 Jul 2022 18:47:49 GMT
VOLUME [/vault/file]
# Mon, 25 Jul 2022 18:47:50 GMT
EXPOSE 8200
# Mon, 25 Jul 2022 18:47:52 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jul 2022 18:47:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jul 2022 18:47:53 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:f4bf3852c6ccaad2dedd57347d310f084247a2e202c2fc20f5fa88d921e8510e`  
		Last Modified: Tue, 19 Jul 2022 22:40:44 GMT  
		Size: 2.7 MB (2717747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:821dde4ee72be0b3dce89d78270d36d363ea3cdc77bc7ae57b09a8c9fc0a8f6a`  
		Last Modified: Mon, 25 Jul 2022 18:48:52 GMT  
		Size: 1.2 KB (1237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927bf878fbb2620959ceff5dac81019cb574ee6ca40f63cdba5f11a0821d3723`  
		Last Modified: Mon, 25 Jul 2022 18:49:01 GMT  
		Size: 65.6 MB (65577649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3132cc1cfdff804bd1e1ca50e1311426d2d0903ba08f3185a1ef78e077aba05`  
		Last Modified: Mon, 25 Jul 2022 18:48:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb03e7a5f0bd90fa24e41e353edf9b3857fa8927f41cc652f9d24705deaab2e`  
		Last Modified: Mon, 25 Jul 2022 18:48:52 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.9.8` - linux; 386

```console
$ docker pull vault@sha256:7f2acda7bad43485ce169bf567b86e9328a5fc3e2bc23a802a92c0bc02daf698
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69588212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ffaf44382b0e563cd1336fc6b72291c31b3b075d8802ae3f5982f4a49db4b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:54 GMT
ADD file:fea8a3ba06779852956b0d3a2dd7514ab33217b1fd395231864c443797f077f6 in / 
# Tue, 09 Aug 2022 17:38:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 00:14:23 GMT
ARG VAULT_VERSION=1.9.8
# Wed, 10 Aug 2022 00:14:24 GMT
# ARGS: VAULT_VERSION=1.9.8
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 10 Aug 2022 00:14:33 GMT
# ARGS: VAULT_VERSION=1.9.8
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 10 Aug 2022 00:14:34 GMT
# ARGS: VAULT_VERSION=1.9.8
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 10 Aug 2022 00:14:34 GMT
VOLUME [/vault/logs]
# Wed, 10 Aug 2022 00:14:35 GMT
VOLUME [/vault/file]
# Wed, 10 Aug 2022 00:14:36 GMT
EXPOSE 8200
# Wed, 10 Aug 2022 00:14:38 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 10 Aug 2022 00:14:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 00:14:39 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:2c44f983a875883421e7d5bc471f6437e0e377e6e7343b52c856caee71064d31`  
		Last Modified: Tue, 09 Aug 2022 17:40:01 GMT  
		Size: 2.8 MB (2832612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21da6d980da46914eff574166091421b3de44074196f1f6cb18b3ddabb179516`  
		Last Modified: Wed, 10 Aug 2022 00:16:09 GMT  
		Size: 1.2 KB (1237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afea6a4a1a07649a0e852b59fa81ee90448fecb643f44bacd0c14b425e160c37`  
		Last Modified: Wed, 10 Aug 2022 00:16:22 GMT  
		Size: 66.8 MB (66752396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874d52115b0f5705afd1bb953f96131a7ff387b19cb1e4ade015aeefd2418ac8`  
		Last Modified: Wed, 10 Aug 2022 00:16:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b231867c08a3e9a63c6f81433abbd7c1fa05dc82ffb32000c54181194548c50`  
		Last Modified: Wed, 10 Aug 2022 00:16:09 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:latest`

```console
$ docker pull vault@sha256:9aa645f2ae2963d803dbb7524679950f451fa4456865ff6454d2a8e0adac5e48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:7a238778738551ab26e07ef2c4ac9d9d9e8d393ec9e766301c9b3bb0fa5f2b55
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.5 MB (77492763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22fdc6314051df714eb280680c24524ed01d0ed2eddff1358cc40d528c82579e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:26:51 GMT
ARG VAULT_VERSION=1.11.2
# Wed, 10 Aug 2022 01:26:52 GMT
# ARGS: VAULT_VERSION=1.11.2
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 10 Aug 2022 01:27:00 GMT
# ARGS: VAULT_VERSION=1.11.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 10 Aug 2022 01:27:01 GMT
# ARGS: VAULT_VERSION=1.11.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 10 Aug 2022 01:27:01 GMT
VOLUME [/vault/logs]
# Wed, 10 Aug 2022 01:27:01 GMT
VOLUME [/vault/file]
# Wed, 10 Aug 2022 01:27:01 GMT
EXPOSE 8200
# Wed, 10 Aug 2022 01:27:01 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 10 Aug 2022 01:27:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 01:27:01 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8967aa5130c8a6f6bb7143c8391df393368db6921ab770555efde013985a9d28`  
		Last Modified: Wed, 10 Aug 2022 01:27:51 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db9d0afc6ab490c62cd716176a04cfd75c36714cb67b9e30a2cda0ef0be75f0`  
		Last Modified: Wed, 10 Aug 2022 01:28:01 GMT  
		Size: 74.7 MB (74662006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0119f940dd249e511bdcf111cbe3b317d64b16eaa192d25fb6b9d83326f33acb`  
		Last Modified: Wed, 10 Aug 2022 01:27:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98184bebb2e9dc29170e6960d8239418e57b92f48ef4edd5a62482071df9c373`  
		Last Modified: Wed, 10 Aug 2022 01:27:51 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:f7b36d61ef1e198262a672601f06e50c01800f197876613fe38eeaaf19e6faf8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70252099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4840ff699b78218305dbfaa6f8a4e5e4fd09a28544ecfc18f38ee02b39a7bcdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:50:02 GMT
ADD file:5a22b2130f6fbe534730df1f47715641a45e55845be7f35c3183e2b74ec43397 in / 
# Tue, 19 Jul 2022 22:50:03 GMT
CMD ["/bin/sh"]
# Thu, 04 Aug 2022 00:49:49 GMT
ARG VAULT_VERSION=1.11.2
# Thu, 04 Aug 2022 00:49:50 GMT
# ARGS: VAULT_VERSION=1.11.2
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 04 Aug 2022 00:50:03 GMT
# ARGS: VAULT_VERSION=1.11.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 04 Aug 2022 00:50:04 GMT
# ARGS: VAULT_VERSION=1.11.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 04 Aug 2022 00:50:04 GMT
VOLUME [/vault/logs]
# Thu, 04 Aug 2022 00:50:04 GMT
VOLUME [/vault/file]
# Thu, 04 Aug 2022 00:50:04 GMT
EXPOSE 8200
# Thu, 04 Aug 2022 00:50:05 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 04 Aug 2022 00:50:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 00:50:05 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:7dc1cbfb63ac7071e143ce96f0f140dc30282039f8d0770eaa7ab97eba515639`  
		Last Modified: Tue, 19 Jul 2022 22:51:41 GMT  
		Size: 2.6 MB (2626632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe5d0bab33752d600ccc29fbfe614ed9b77022cc6917e0d105f43029315d5c1`  
		Last Modified: Thu, 04 Aug 2022 00:51:25 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddad393ff0b354750574a05b6092fc9d6af3767312789455a8e557815014dca`  
		Last Modified: Thu, 04 Aug 2022 00:51:38 GMT  
		Size: 67.6 MB (67622196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4fd1bd01fd74ec5a209c0e8ef421017bbc7c6710c69b8167bb4973fbd35d84`  
		Last Modified: Thu, 04 Aug 2022 00:51:25 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8aa266ce16913028810350646722976666d954374379b285b0f65ba4337da8`  
		Last Modified: Thu, 04 Aug 2022 00:51:25 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:a5e9ea80e35ff247cf83cc7ab06022c50366d7e36ec1135e4d740b7496bb201e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72280976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74e752c8d20377f9028c78a12d70d10ac833656174e6e64c9df558a3e5a0655d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:39:51 GMT
ADD file:bb30934245445dabbe698387b5d454c2360d05055f7ab1bcaaffefea5aefb539 in / 
# Tue, 19 Jul 2022 22:39:51 GMT
CMD ["/bin/sh"]
# Thu, 04 Aug 2022 00:42:15 GMT
ARG VAULT_VERSION=1.11.2
# Thu, 04 Aug 2022 00:42:16 GMT
# ARGS: VAULT_VERSION=1.11.2
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 04 Aug 2022 00:42:25 GMT
# ARGS: VAULT_VERSION=1.11.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 04 Aug 2022 00:42:26 GMT
# ARGS: VAULT_VERSION=1.11.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 04 Aug 2022 00:42:26 GMT
VOLUME [/vault/logs]
# Thu, 04 Aug 2022 00:42:27 GMT
VOLUME [/vault/file]
# Thu, 04 Aug 2022 00:42:28 GMT
EXPOSE 8200
# Thu, 04 Aug 2022 00:42:30 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 04 Aug 2022 00:42:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 00:42:31 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:f4bf3852c6ccaad2dedd57347d310f084247a2e202c2fc20f5fa88d921e8510e`  
		Last Modified: Tue, 19 Jul 2022 22:40:44 GMT  
		Size: 2.7 MB (2717747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b09458246504b8537fdc40489d178a1162f42ae33f83d1668f22dbbb02618d`  
		Last Modified: Thu, 04 Aug 2022 00:43:02 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f72f8bcd3c8ec0587c1e140832995309ee204e3156ecf582e9837f3eb65f64`  
		Last Modified: Thu, 04 Aug 2022 00:43:10 GMT  
		Size: 69.6 MB (69560017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0db6c642a591863aed2683b2e9bc4e30ceb7f6d2a809fe973dc200c155bfd8d`  
		Last Modified: Thu, 04 Aug 2022 00:43:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493a5d945bb81c3d49c8e11b278e072bc4f9df393039f72357a332239acf4672`  
		Last Modified: Thu, 04 Aug 2022 00:43:02 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:556137692bc84155dc5886a12ae852d4ce1d5bb058e207d43a07f5ce716f0808
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73567722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9c7a4e16b968a99b1ef223d5cde6b79ad51103581802e72741be70c9ea5db3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:54 GMT
ADD file:fea8a3ba06779852956b0d3a2dd7514ab33217b1fd395231864c443797f077f6 in / 
# Tue, 09 Aug 2022 17:38:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 00:13:39 GMT
ARG VAULT_VERSION=1.11.2
# Wed, 10 Aug 2022 00:13:40 GMT
# ARGS: VAULT_VERSION=1.11.2
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 10 Aug 2022 00:13:49 GMT
# ARGS: VAULT_VERSION=1.11.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 10 Aug 2022 00:13:50 GMT
# ARGS: VAULT_VERSION=1.11.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 10 Aug 2022 00:13:51 GMT
VOLUME [/vault/logs]
# Wed, 10 Aug 2022 00:13:52 GMT
VOLUME [/vault/file]
# Wed, 10 Aug 2022 00:13:53 GMT
EXPOSE 8200
# Wed, 10 Aug 2022 00:13:55 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 10 Aug 2022 00:13:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 00:13:56 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:2c44f983a875883421e7d5bc471f6437e0e377e6e7343b52c856caee71064d31`  
		Last Modified: Tue, 09 Aug 2022 17:40:01 GMT  
		Size: 2.8 MB (2832612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fdb4858833cdfc5a5714d5a19c93b337a0e778ec7d80ef77189fac0471c7566`  
		Last Modified: Wed, 10 Aug 2022 00:15:25 GMT  
		Size: 1.2 KB (1237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb24cb72e1a2fdb06de8d1a5f75cd0a549f107b77909b2a0c1b20f9e2d74d29`  
		Last Modified: Wed, 10 Aug 2022 00:15:36 GMT  
		Size: 70.7 MB (70731906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7744188d2a7166aef058bb6d424153beba212e4c8749f465cf86914a226ca7`  
		Last Modified: Wed, 10 Aug 2022 00:15:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90460ac0bbb803713f9962bf787cb7021494e0163af9926e3ac5956d65c240d`  
		Last Modified: Wed, 10 Aug 2022 00:15:25 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
