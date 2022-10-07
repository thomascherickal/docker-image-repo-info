<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:1.10.6`](#vault1106)
-	[`vault:1.11.3`](#vault1113)
-	[`vault:1.8.12`](#vault1812)
-	[`vault:1.9.9`](#vault199)
-	[`vault:latest`](#vaultlatest)

## `vault:1.10.6`

```console
$ docker pull vault@sha256:646f52f7a4e28c724e0225cae306fc4e0500a6f3f84780f3d3ef311a885a725f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.10.6` - linux; amd64

```console
$ docker pull vault@sha256:8d9de4db20deb53e4a603e6eb624c64eeba5fd847b180212e87739f2df4674ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74105607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:817cab5c1340ff202000a7ac3d0f12c808549ef99024deb0041c247ec7ead236`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:27:25 GMT
ARG VAULT_VERSION=1.10.6
# Fri, 07 Oct 2022 04:27:26 GMT
# ARGS: VAULT_VERSION=1.10.6
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 07 Oct 2022 04:27:34 GMT
# ARGS: VAULT_VERSION=1.10.6
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 07 Oct 2022 04:27:35 GMT
# ARGS: VAULT_VERSION=1.10.6
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 07 Oct 2022 04:27:35 GMT
VOLUME [/vault/logs]
# Fri, 07 Oct 2022 04:27:35 GMT
VOLUME [/vault/file]
# Fri, 07 Oct 2022 04:27:35 GMT
EXPOSE 8200
# Fri, 07 Oct 2022 04:27:36 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 07 Oct 2022 04:27:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 04:27:36 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cf65614942d7153bd2ec257e9ef4da85206176e23cc2276fd8f67bc51f3b17`  
		Last Modified: Fri, 07 Oct 2022 04:28:31 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dda55ca13436e87ceedeba0bbbb7ceefd3c927ce9b630b8e22022ddba52b17`  
		Last Modified: Fri, 07 Oct 2022 04:28:39 GMT  
		Size: 71.3 MB (71274848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488bae8cf384f34733467e417cc22d239536f5eb21d41e6953134569126b0887`  
		Last Modified: Fri, 07 Oct 2022 04:28:31 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553207aeb1923eb22420f7d0d7aee94c019831966de11c8e3bd1dafa1d1a07bd`  
		Last Modified: Fri, 07 Oct 2022 04:28:31 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.10.6` - linux; arm variant v6

```console
$ docker pull vault@sha256:66276b6b00a13a10e69141715bc66327313c4ae099a93884f3e7962de40cbc03
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67355776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccad3e6f6d0f8dae0186409b20c543b058a55559b5b10420a4519d85dde659ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:35 GMT
ADD file:8ff80989f06f5a8ffe16c56e00538928dcb1e46faa2b58ab9c14c7227a6cd8f9 in / 
# Tue, 09 Aug 2022 17:49:35 GMT
CMD ["/bin/sh"]
# Wed, 31 Aug 2022 21:50:02 GMT
ARG VAULT_VERSION=1.10.6
# Wed, 31 Aug 2022 21:50:02 GMT
# ARGS: VAULT_VERSION=1.10.6
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 31 Aug 2022 21:50:11 GMT
# ARGS: VAULT_VERSION=1.10.6
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 31 Aug 2022 21:50:12 GMT
# ARGS: VAULT_VERSION=1.10.6
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 31 Aug 2022 21:50:12 GMT
VOLUME [/vault/logs]
# Wed, 31 Aug 2022 21:50:12 GMT
VOLUME [/vault/file]
# Wed, 31 Aug 2022 21:50:12 GMT
EXPOSE 8200
# Wed, 31 Aug 2022 21:50:12 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 31 Aug 2022 21:50:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Aug 2022 21:50:12 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:7d147289082e6aa6ef510c09d7c0ac8b5026e0b591f1bfcaf01ceada43c9ec65`  
		Last Modified: Tue, 09 Aug 2022 17:51:04 GMT  
		Size: 2.6 MB (2635498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2359565337ce1bf9326291a3d8c34a82bc1284d78de680065dcf09721adce658`  
		Last Modified: Wed, 31 Aug 2022 21:51:10 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8a682c1df3b03f18942c2a9328c8ca3e24b358590902bf08422c54ef1a0716`  
		Last Modified: Wed, 31 Aug 2022 21:51:19 GMT  
		Size: 64.7 MB (64717006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7a6e62a09e5a3eb430dc9286d9701097148d8f8af2f906d0e0c44374fb5de6`  
		Last Modified: Wed, 31 Aug 2022 21:51:10 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea95041b272f04a12e007b18fcbc0451bf31bdc2221066e69529c2658c6d177`  
		Last Modified: Wed, 31 Aug 2022 21:51:10 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.10.6` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:ba95e606582dc5f339886a1837b43b39b4a703767e6f1a53b2216d4962f9b902
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69166256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46994eee1b860917526c9d0f583aef84896e97a94ff1ef8e7f6d3b20dc6999f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:59 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Tue, 09 Aug 2022 17:39:59 GMT
CMD ["/bin/sh"]
# Wed, 31 Aug 2022 21:47:23 GMT
ARG VAULT_VERSION=1.10.6
# Wed, 31 Aug 2022 21:47:23 GMT
# ARGS: VAULT_VERSION=1.10.6
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 31 Aug 2022 21:47:35 GMT
# ARGS: VAULT_VERSION=1.10.6
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 31 Aug 2022 21:47:36 GMT
# ARGS: VAULT_VERSION=1.10.6
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 31 Aug 2022 21:47:37 GMT
VOLUME [/vault/logs]
# Wed, 31 Aug 2022 21:47:38 GMT
VOLUME [/vault/file]
# Wed, 31 Aug 2022 21:47:39 GMT
EXPOSE 8200
# Wed, 31 Aug 2022 21:47:41 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 31 Aug 2022 21:47:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Aug 2022 21:47:42 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a2c1f4531f4ca8a103761917c8f98cd72aa2b43ce2005ad8cc45545978513f`  
		Last Modified: Wed, 31 Aug 2022 21:48:44 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f810f933052643bbb96e984a3c2760d0bfe16ffa7175b33ff2f2b3e95a131ddc`  
		Last Modified: Wed, 31 Aug 2022 21:48:52 GMT  
		Size: 66.4 MB (66440892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8d93f12c8b6a404a69ceb4ab4f570a1dde3208b708c20f100433be011059dc`  
		Last Modified: Wed, 31 Aug 2022 21:48:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a473a297e59c4fb01204dc430edd393f979a9a8c4c36a0fd2a79020055109d9`  
		Last Modified: Wed, 31 Aug 2022 21:48:44 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.10.6` - linux; 386

```console
$ docker pull vault@sha256:b35675ff90c9b1f4a4b23d5a523c06d7087f02cbf563f2b378a62dc71e3272a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.5 MB (70453865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48b46b8937333ddedd42183b88d3b4359eb1a6a0437a9d0581a9131e76050712`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:54 GMT
ADD file:fea8a3ba06779852956b0d3a2dd7514ab33217b1fd395231864c443797f077f6 in / 
# Tue, 09 Aug 2022 17:38:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 02:17:02 GMT
ARG VAULT_VERSION=1.10.6
# Fri, 07 Oct 2022 02:17:03 GMT
# ARGS: VAULT_VERSION=1.10.6
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 07 Oct 2022 02:17:11 GMT
# ARGS: VAULT_VERSION=1.10.6
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 07 Oct 2022 02:17:12 GMT
# ARGS: VAULT_VERSION=1.10.6
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 07 Oct 2022 02:17:13 GMT
VOLUME [/vault/logs]
# Fri, 07 Oct 2022 02:17:14 GMT
VOLUME [/vault/file]
# Fri, 07 Oct 2022 02:17:15 GMT
EXPOSE 8200
# Fri, 07 Oct 2022 02:17:17 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 07 Oct 2022 02:17:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 02:17:18 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:2c44f983a875883421e7d5bc471f6437e0e377e6e7343b52c856caee71064d31`  
		Last Modified: Tue, 09 Aug 2022 17:40:01 GMT  
		Size: 2.8 MB (2832612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a639156565d26031c1d0da850edd2d47ea8116cefaba2d5262322a89a3d28037`  
		Last Modified: Fri, 07 Oct 2022 02:18:42 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12db1524c2363d8ae1bcb5ec72a266ed7781bf167e7152d45d82f2a44e8c55d9`  
		Last Modified: Fri, 07 Oct 2022 02:18:50 GMT  
		Size: 67.6 MB (67618046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26fdcdcec3596105f04383f3607655503fc6bbd0d2db7332f20b93aded0f24f`  
		Last Modified: Fri, 07 Oct 2022 02:18:42 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf7999115cc2c36db6c1a042c1162b4c0be88c6225a4c1c886dff75876444f2`  
		Last Modified: Fri, 07 Oct 2022 02:18:42 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.11.3`

```console
$ docker pull vault@sha256:df304a65c19053d7b2f289fa71dd037392f8143ac2d3921599aa47d11b777692
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.11.3` - linux; amd64

```console
$ docker pull vault@sha256:e0c328735ebffece80997b81e68c55352b3ae5dbd792b01808a5b11dada01a73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.6 MB (77566729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31a577a370a4eb69838201f06f24feb4d0e2e707ac6db2c707bad9ea405e1db1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:27:12 GMT
ARG VAULT_VERSION=1.11.3
# Fri, 07 Oct 2022 04:27:12 GMT
# ARGS: VAULT_VERSION=1.11.3
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 07 Oct 2022 04:27:20 GMT
# ARGS: VAULT_VERSION=1.11.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 07 Oct 2022 04:27:21 GMT
# ARGS: VAULT_VERSION=1.11.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 07 Oct 2022 04:27:21 GMT
VOLUME [/vault/logs]
# Fri, 07 Oct 2022 04:27:22 GMT
VOLUME [/vault/file]
# Fri, 07 Oct 2022 04:27:22 GMT
EXPOSE 8200
# Fri, 07 Oct 2022 04:27:22 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 07 Oct 2022 04:27:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 04:27:22 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33abb1f4412ecd617c25a888039e5e95e9591e4477a535bdf4eb9f639a0a03c6`  
		Last Modified: Fri, 07 Oct 2022 04:28:12 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fccdaef23ddba75b8b22e8df726571a4887aea1eca291fc60ca0464e7504ca9`  
		Last Modified: Fri, 07 Oct 2022 04:28:22 GMT  
		Size: 74.7 MB (74735969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e018fbf02db00931d824e80d70381413695ff777c20d8270acfb156e28d45e57`  
		Last Modified: Fri, 07 Oct 2022 04:28:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb84ed27959e103f1bfb81362c25b5472fe796cc66ff99a777b68d583298358`  
		Last Modified: Fri, 07 Oct 2022 04:28:13 GMT  
		Size: 1.8 KB (1816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.11.3` - linux; arm variant v6

```console
$ docker pull vault@sha256:f30429e9665d0b870af7613514b22d09eb8e3312c3a769b994c02e0f5ba71470
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70297307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06c4fd3ece3522b64385b01c48ce3cfbb24327af74b6048a23987ea1094d8324`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:35 GMT
ADD file:8ff80989f06f5a8ffe16c56e00538928dcb1e46faa2b58ab9c14c7227a6cd8f9 in / 
# Tue, 09 Aug 2022 17:49:35 GMT
CMD ["/bin/sh"]
# Wed, 31 Aug 2022 21:49:43 GMT
ARG VAULT_VERSION=1.11.3
# Wed, 31 Aug 2022 21:49:44 GMT
# ARGS: VAULT_VERSION=1.11.3
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 31 Aug 2022 21:49:55 GMT
# ARGS: VAULT_VERSION=1.11.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 31 Aug 2022 21:49:56 GMT
# ARGS: VAULT_VERSION=1.11.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 31 Aug 2022 21:49:56 GMT
VOLUME [/vault/logs]
# Wed, 31 Aug 2022 21:49:56 GMT
VOLUME [/vault/file]
# Wed, 31 Aug 2022 21:49:56 GMT
EXPOSE 8200
# Wed, 31 Aug 2022 21:49:57 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 31 Aug 2022 21:49:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Aug 2022 21:49:57 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:7d147289082e6aa6ef510c09d7c0ac8b5026e0b591f1bfcaf01ceada43c9ec65`  
		Last Modified: Tue, 09 Aug 2022 17:51:04 GMT  
		Size: 2.6 MB (2635498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914e9b4e0991feb43a7b6f4386db37552134233dba7d7e67509e026532e3fc78`  
		Last Modified: Wed, 31 Aug 2022 21:50:50 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191451985f0bf67d8569b41d9eff27bcb25554427eae1c47670635c691828043`  
		Last Modified: Wed, 31 Aug 2022 21:50:59 GMT  
		Size: 67.7 MB (67658537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3e767244b4a31c1ffa01bef811242d0067e732938c98d6b2b73fe55aa3857c`  
		Last Modified: Wed, 31 Aug 2022 21:50:50 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc3cf4938d7600d2fb9408f0b8c6a7b5521f89393695eaf7e8aad62dcc8fbb1`  
		Last Modified: Wed, 31 Aug 2022 21:50:50 GMT  
		Size: 1.8 KB (1816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.11.3` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:7f067bb99986c4f0b7449ff9002f1456900f3c3dc5211939d0fc20a6b8287049
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72347537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7847c948d0303e222e446d85168c3b8b31fbf268f0efa3b3875998fefbff994`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:59 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Tue, 09 Aug 2022 17:39:59 GMT
CMD ["/bin/sh"]
# Wed, 31 Aug 2022 21:47:00 GMT
ARG VAULT_VERSION=1.11.3
# Wed, 31 Aug 2022 21:47:01 GMT
# ARGS: VAULT_VERSION=1.11.3
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 31 Aug 2022 21:47:10 GMT
# ARGS: VAULT_VERSION=1.11.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 31 Aug 2022 21:47:10 GMT
# ARGS: VAULT_VERSION=1.11.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 31 Aug 2022 21:47:11 GMT
VOLUME [/vault/logs]
# Wed, 31 Aug 2022 21:47:12 GMT
VOLUME [/vault/file]
# Wed, 31 Aug 2022 21:47:13 GMT
EXPOSE 8200
# Wed, 31 Aug 2022 21:47:15 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 31 Aug 2022 21:47:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Aug 2022 21:47:16 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef99c9689f07239e0f31a674f13b44e6c80a58182364a3e63c8b1c2af076def1`  
		Last Modified: Wed, 31 Aug 2022 21:48:24 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa2627c8cbee16d9c343f5e884d1e030a26236180d214ca357c13f97c036386`  
		Last Modified: Wed, 31 Aug 2022 21:48:33 GMT  
		Size: 69.6 MB (69622173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45314dd300cb3b4ff0a157e3c3053fd52106832568455081a8b37353c75aea5`  
		Last Modified: Wed, 31 Aug 2022 21:48:24 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08ff4ca234e6c92871957ff044a4a8351918e7f06b609334b4caed4528745a2`  
		Last Modified: Wed, 31 Aug 2022 21:48:24 GMT  
		Size: 1.8 KB (1818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.11.3` - linux; 386

```console
$ docker pull vault@sha256:1b34b6fda393d8a334c4eedc0b175131fc942884cdcca602dd43aaf5837fb797
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73616298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99a14805e808dea6ba008321458115e9beb278026cdc686886e13ca32edc87fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:54 GMT
ADD file:fea8a3ba06779852956b0d3a2dd7514ab33217b1fd395231864c443797f077f6 in / 
# Tue, 09 Aug 2022 17:38:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 02:16:39 GMT
ARG VAULT_VERSION=1.11.3
# Fri, 07 Oct 2022 02:16:40 GMT
# ARGS: VAULT_VERSION=1.11.3
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 07 Oct 2022 02:16:49 GMT
# ARGS: VAULT_VERSION=1.11.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 07 Oct 2022 02:16:50 GMT
# ARGS: VAULT_VERSION=1.11.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 07 Oct 2022 02:16:51 GMT
VOLUME [/vault/logs]
# Fri, 07 Oct 2022 02:16:52 GMT
VOLUME [/vault/file]
# Fri, 07 Oct 2022 02:16:53 GMT
EXPOSE 8200
# Fri, 07 Oct 2022 02:16:55 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 07 Oct 2022 02:16:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 02:16:56 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:2c44f983a875883421e7d5bc471f6437e0e377e6e7343b52c856caee71064d31`  
		Last Modified: Tue, 09 Aug 2022 17:40:01 GMT  
		Size: 2.8 MB (2832612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b10cbdcb59e9628ceffee1669ab783814ef5732d48fd26a88e0b81b3ebb76f`  
		Last Modified: Fri, 07 Oct 2022 02:18:23 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0021f9d2571bc9ba83476d8a0d830aee98a1b7700bc85711a8952951e9c37503`  
		Last Modified: Fri, 07 Oct 2022 02:18:30 GMT  
		Size: 70.8 MB (70780476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a9c4b0a196d9edaa84d26b358a70533e825c3f077842d4b303817245815f20c`  
		Last Modified: Fri, 07 Oct 2022 02:18:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99cb0f64666b4642358204e21488ada2f7edad88fc7f9bf08a3b09be324e9ef2`  
		Last Modified: Fri, 07 Oct 2022 02:18:23 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.8.12`

```console
$ docker pull vault@sha256:97035037e200f5920400c3b8fc75d8df12f91ccdb82e5bef6755513b5d67f0a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.8.12` - linux; amd64

```console
$ docker pull vault@sha256:93c497e4e559599e8a098e1aa0a6db4c939a69c3ec5e2678cc3e5d80e3ae8cf8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70643377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:499350482e03b8dda3e27354df763b7dcdbcabe305acb1c66c9b87384936b87c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:27:53 GMT
ARG VAULT_VERSION=1.8.12
# Fri, 07 Oct 2022 04:27:54 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 07 Oct 2022 04:28:01 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 07 Oct 2022 04:28:02 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 07 Oct 2022 04:28:02 GMT
VOLUME [/vault/logs]
# Fri, 07 Oct 2022 04:28:02 GMT
VOLUME [/vault/file]
# Fri, 07 Oct 2022 04:28:02 GMT
EXPOSE 8200
# Fri, 07 Oct 2022 04:28:02 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 07 Oct 2022 04:28:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 04:28:03 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc1ed5fcb6f5bccca2a500778dc34f4bf75f207aabb55e910ae839c69105d16`  
		Last Modified: Fri, 07 Oct 2022 04:29:02 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f865244d5ec4b3bdb123510f617888b8c9f2a86c9eb02b7d1053329bf050c26b`  
		Last Modified: Fri, 07 Oct 2022 04:29:11 GMT  
		Size: 67.8 MB (67812617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b94e74664deec379ff512c03ed5a69be5d82f336696257a900817a1b7549b56`  
		Last Modified: Fri, 07 Oct 2022 04:29:02 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ab1cc8b564b14383c667ff287feff7508c198eb608e45170732ddf07b6da5f`  
		Last Modified: Fri, 07 Oct 2022 04:29:02 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.8.12` - linux; arm variant v6

```console
$ docker pull vault@sha256:df35696f78627af5c87335be699c09c3aaba3b57e88405a60339ff72ee87391b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (64979329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b06af3699f89f815b16584b7140b34663df5a4b2abdd3d1bb61d4f00560294`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:35 GMT
ADD file:8ff80989f06f5a8ffe16c56e00538928dcb1e46faa2b58ab9c14c7227a6cd8f9 in / 
# Tue, 09 Aug 2022 17:49:35 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:39:18 GMT
ARG VAULT_VERSION=1.8.12
# Thu, 11 Aug 2022 00:39:19 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 11 Aug 2022 00:39:27 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 11 Aug 2022 00:39:27 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 11 Aug 2022 00:39:27 GMT
VOLUME [/vault/logs]
# Thu, 11 Aug 2022 00:39:27 GMT
VOLUME [/vault/file]
# Thu, 11 Aug 2022 00:39:28 GMT
EXPOSE 8200
# Thu, 11 Aug 2022 00:39:28 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 11 Aug 2022 00:39:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 00:39:28 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:7d147289082e6aa6ef510c09d7c0ac8b5026e0b591f1bfcaf01ceada43c9ec65`  
		Last Modified: Tue, 09 Aug 2022 17:51:04 GMT  
		Size: 2.6 MB (2635498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80507948872f98adb21bf90308df85f8f14fd6bf78b494048a1c2df54173107e`  
		Last Modified: Thu, 11 Aug 2022 00:40:41 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ee86e3c44c3a78d335c6dba79086c6a17794fd6688ab976211e81635162be7`  
		Last Modified: Thu, 11 Aug 2022 00:40:49 GMT  
		Size: 62.3 MB (62340561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a18fa6d1ca7c11d0fa8d02521be3cbeb32f9ec098c947ba89f236c7a96e880`  
		Last Modified: Thu, 11 Aug 2022 00:40:42 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dfa1d16b2af971034dc6975b6af3c8c26b534193b95ffdda15f7a42e8351b02`  
		Last Modified: Thu, 11 Aug 2022 00:40:41 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.8.12` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:af9f850ac3772bc779d576ba64da9b1f56ee557f057dd2ebb2c32f101de83a28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66912119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7756cfd35375d5a8f6af3ba87bbfa6bb7bc6dce28aa686c8de4282ccf2eecf4c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:59 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Tue, 09 Aug 2022 17:39:59 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:22:40 GMT
ARG VAULT_VERSION=1.8.12
# Wed, 10 Aug 2022 06:22:41 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 10 Aug 2022 06:22:49 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 10 Aug 2022 06:22:49 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 10 Aug 2022 06:22:50 GMT
VOLUME [/vault/logs]
# Wed, 10 Aug 2022 06:22:51 GMT
VOLUME [/vault/file]
# Wed, 10 Aug 2022 06:22:52 GMT
EXPOSE 8200
# Wed, 10 Aug 2022 06:22:54 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 10 Aug 2022 06:22:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 06:22:55 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4ff73e0df6cdb90ca1a83460da75b2cb653a02ea996b9c4acc2d7b36d6c475`  
		Last Modified: Wed, 10 Aug 2022 06:24:11 GMT  
		Size: 1.2 KB (1237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e382d9dd47cfcba359cb759708414caaf1880e8e5afa9a5a365da38b2213232c`  
		Last Modified: Wed, 10 Aug 2022 06:24:19 GMT  
		Size: 64.2 MB (64186762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cec19ed89bb76bae1a3f36b5772229e77d13589beb6ba54f0bb6987dfaeef9`  
		Last Modified: Wed, 10 Aug 2022 06:24:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4ebac347c03ab4322d1931725e558a8b0dbdedff1eeeb637fbdf869343f7f1`  
		Last Modified: Wed, 10 Aug 2022 06:24:11 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.8.12` - linux; 386

```console
$ docker pull vault@sha256:166b6f4c5c7d7c7e5947c9b763e9346b472cdf7d866180c50ca8ad9381600390
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68342143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf90b1387227b78022082504e177a361bdc6fa70d900782a847d341eeb75ed4c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:54 GMT
ADD file:fea8a3ba06779852956b0d3a2dd7514ab33217b1fd395231864c443797f077f6 in / 
# Tue, 09 Aug 2022 17:38:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 02:17:46 GMT
ARG VAULT_VERSION=1.8.12
# Fri, 07 Oct 2022 02:17:47 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 07 Oct 2022 02:17:56 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 07 Oct 2022 02:17:57 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 07 Oct 2022 02:17:58 GMT
VOLUME [/vault/logs]
# Fri, 07 Oct 2022 02:17:59 GMT
VOLUME [/vault/file]
# Fri, 07 Oct 2022 02:18:00 GMT
EXPOSE 8200
# Fri, 07 Oct 2022 02:18:02 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 07 Oct 2022 02:18:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 02:18:03 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:2c44f983a875883421e7d5bc471f6437e0e377e6e7343b52c856caee71064d31`  
		Last Modified: Tue, 09 Aug 2022 17:40:01 GMT  
		Size: 2.8 MB (2832612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84de5fc98a8d687a958eb5d004e3e3804a3b4f3fbfa4f610cbeb6cdb3ab0614`  
		Last Modified: Fri, 07 Oct 2022 02:19:12 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7bbf9c104d2287ba3ee86e365d27c7bdb93d752ce013fa85dfa47e801f00cf`  
		Last Modified: Fri, 07 Oct 2022 02:19:19 GMT  
		Size: 65.5 MB (65506322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd8b373c5f3620bbb4dd0a6a8806a84e52a656cc6db68b9672d022d0854217a`  
		Last Modified: Fri, 07 Oct 2022 02:19:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb2e8cd94e55cd548f859261a1476700cd0af7e893546f54437a848300ee92e`  
		Last Modified: Fri, 07 Oct 2022 02:19:12 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.9.9`

```console
$ docker pull vault@sha256:38174d22dd28d29ea1902b2836de54ddc9f16050c510a5bfba1c97a1b58324fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.9.9` - linux; amd64

```console
$ docker pull vault@sha256:4825a6933b9d5da70cbdbde1e901d59bff3b15812242bedf30f9fc67ea7e2cc7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73212978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29e97da9098de8d3a08a491c5ac11e3d32303c7234d3965b83fbb747cb7f842e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:27:39 GMT
ARG VAULT_VERSION=1.9.9
# Fri, 07 Oct 2022 04:27:41 GMT
# ARGS: VAULT_VERSION=1.9.9
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 07 Oct 2022 04:27:49 GMT
# ARGS: VAULT_VERSION=1.9.9
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 07 Oct 2022 04:27:50 GMT
# ARGS: VAULT_VERSION=1.9.9
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 07 Oct 2022 04:27:50 GMT
VOLUME [/vault/logs]
# Fri, 07 Oct 2022 04:27:50 GMT
VOLUME [/vault/file]
# Fri, 07 Oct 2022 04:27:50 GMT
EXPOSE 8200
# Fri, 07 Oct 2022 04:27:50 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 07 Oct 2022 04:27:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 04:27:51 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab98be999987140e3f58f331e9f5c1f5d771da2cd21ac9015d4e60092617a6c`  
		Last Modified: Fri, 07 Oct 2022 04:28:46 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a032485917c2916a0208d8e81765baaed9235f8feeacc3a556319f9c32cc0d`  
		Last Modified: Fri, 07 Oct 2022 04:28:55 GMT  
		Size: 70.4 MB (70382216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b76fcee5c45417e007b9d7c5aa491bc0adc2ccfcee9db558247eb618dde2e6b`  
		Last Modified: Fri, 07 Oct 2022 04:28:46 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e338c5e53cb36ca3c16cd8a70851812a7d283c04c1203e462922afc8f3c879`  
		Last Modified: Fri, 07 Oct 2022 04:28:46 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.9.9` - linux; arm variant v6

```console
$ docker pull vault@sha256:d3746ead42e7b12f20badd216f76cc05dc8c87015f7bcbfcb2f9a00a539ec924
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66525164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13c0f94a761f2202a7a8665e2df6c89f7d76a72684c2f3fc8042d97a6fae8f89`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:35 GMT
ADD file:8ff80989f06f5a8ffe16c56e00538928dcb1e46faa2b58ab9c14c7227a6cd8f9 in / 
# Tue, 09 Aug 2022 17:49:35 GMT
CMD ["/bin/sh"]
# Wed, 31 Aug 2022 21:50:17 GMT
ARG VAULT_VERSION=1.9.9
# Wed, 31 Aug 2022 21:50:17 GMT
# ARGS: VAULT_VERSION=1.9.9
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 31 Aug 2022 21:50:26 GMT
# ARGS: VAULT_VERSION=1.9.9
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 31 Aug 2022 21:50:27 GMT
# ARGS: VAULT_VERSION=1.9.9
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 31 Aug 2022 21:50:27 GMT
VOLUME [/vault/logs]
# Wed, 31 Aug 2022 21:50:27 GMT
VOLUME [/vault/file]
# Wed, 31 Aug 2022 21:50:27 GMT
EXPOSE 8200
# Wed, 31 Aug 2022 21:50:27 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 31 Aug 2022 21:50:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Aug 2022 21:50:28 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:7d147289082e6aa6ef510c09d7c0ac8b5026e0b591f1bfcaf01ceada43c9ec65`  
		Last Modified: Tue, 09 Aug 2022 17:51:04 GMT  
		Size: 2.6 MB (2635498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d90356eb05e04fdead1bc8f44af1533ae40301d250d0a3a3f9631ea26c2af23`  
		Last Modified: Wed, 31 Aug 2022 21:51:27 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5f8b05fc7a830e4e6c53c8fe1167bb4014751b08b5e79cd445822e9529314cf`  
		Last Modified: Wed, 31 Aug 2022 21:51:36 GMT  
		Size: 63.9 MB (63886396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be61404b7b8416b372c79d6053dadf69f90535ebc12ab0930d97aff288720f76`  
		Last Modified: Wed, 31 Aug 2022 21:51:27 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ac56dfa64e71e02c3be903cea647fee4a8f28f78e72fa626396d0e0c291a59`  
		Last Modified: Wed, 31 Aug 2022 21:51:27 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.9.9` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:33e17a911176ec42091b1ccf035ce45f32c9506c7eefae0d0cd7d247e27b298e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68321777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aeefe6c69a175b768b0c8d60963ff933e72f07527f633f2e4b9fb56bc427af1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:59 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Tue, 09 Aug 2022 17:39:59 GMT
CMD ["/bin/sh"]
# Wed, 31 Aug 2022 21:47:49 GMT
ARG VAULT_VERSION=1.9.9
# Wed, 31 Aug 2022 21:47:50 GMT
# ARGS: VAULT_VERSION=1.9.9
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 31 Aug 2022 21:47:57 GMT
# ARGS: VAULT_VERSION=1.9.9
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 31 Aug 2022 21:47:58 GMT
# ARGS: VAULT_VERSION=1.9.9
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 31 Aug 2022 21:47:59 GMT
VOLUME [/vault/logs]
# Wed, 31 Aug 2022 21:48:00 GMT
VOLUME [/vault/file]
# Wed, 31 Aug 2022 21:48:01 GMT
EXPOSE 8200
# Wed, 31 Aug 2022 21:48:03 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 31 Aug 2022 21:48:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Aug 2022 21:48:04 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb03582acd9ddc7afbfbeb6b25d957db425d1f7e9f22fb49faaee952b1e38434`  
		Last Modified: Wed, 31 Aug 2022 21:49:01 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028951928a309eef1ade63ea3753da6a5bde40d95d959a1b1c7d024d56ab1987`  
		Last Modified: Wed, 31 Aug 2022 21:49:09 GMT  
		Size: 65.6 MB (65596414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42bb747a679454743b5ff4e32389ff51d0a89455a554df2f5ab6efaf4df28be`  
		Last Modified: Wed, 31 Aug 2022 21:49:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd825f92fea57253d563a87382a717f1050f67e8bcc8289917efb5cdd0b916c`  
		Last Modified: Wed, 31 Aug 2022 21:49:00 GMT  
		Size: 1.8 KB (1816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.9.9` - linux; 386

```console
$ docker pull vault@sha256:d8544a043531b375a88dabf6dbd6ab2b9669b43127869278620800b204d6fb82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69575850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d55555a0de20c4023b67a99ce9fb30745e13d9de2d111d71db4bca51e3690f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:54 GMT
ADD file:fea8a3ba06779852956b0d3a2dd7514ab33217b1fd395231864c443797f077f6 in / 
# Tue, 09 Aug 2022 17:38:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 02:17:24 GMT
ARG VAULT_VERSION=1.9.9
# Fri, 07 Oct 2022 02:17:25 GMT
# ARGS: VAULT_VERSION=1.9.9
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 07 Oct 2022 02:17:34 GMT
# ARGS: VAULT_VERSION=1.9.9
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 07 Oct 2022 02:17:34 GMT
# ARGS: VAULT_VERSION=1.9.9
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 07 Oct 2022 02:17:35 GMT
VOLUME [/vault/logs]
# Fri, 07 Oct 2022 02:17:36 GMT
VOLUME [/vault/file]
# Fri, 07 Oct 2022 02:17:37 GMT
EXPOSE 8200
# Fri, 07 Oct 2022 02:17:39 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 07 Oct 2022 02:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 02:17:40 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:2c44f983a875883421e7d5bc471f6437e0e377e6e7343b52c856caee71064d31`  
		Last Modified: Tue, 09 Aug 2022 17:40:01 GMT  
		Size: 2.8 MB (2832612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be51e1476878e2229fa15eb735d4ac877a615282d5fc305837eaf90a5d7c3190`  
		Last Modified: Fri, 07 Oct 2022 02:18:57 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abefb575794504891b6fb7b3ae77dc7a5c40861b2c93620f0290eaa475e78043`  
		Last Modified: Fri, 07 Oct 2022 02:19:04 GMT  
		Size: 66.7 MB (66740026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae85b854a95df6733b395355efc7eb76da596b984507d079d7225e5df032e04`  
		Last Modified: Fri, 07 Oct 2022 02:18:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b92bb22c95721f7cc2080896eeb68c8d1700468893e890ec66a58c4396e481`  
		Last Modified: Fri, 07 Oct 2022 02:18:57 GMT  
		Size: 1.8 KB (1816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:latest`

```console
$ docker pull vault@sha256:df304a65c19053d7b2f289fa71dd037392f8143ac2d3921599aa47d11b777692
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:e0c328735ebffece80997b81e68c55352b3ae5dbd792b01808a5b11dada01a73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.6 MB (77566729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31a577a370a4eb69838201f06f24feb4d0e2e707ac6db2c707bad9ea405e1db1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:27:12 GMT
ARG VAULT_VERSION=1.11.3
# Fri, 07 Oct 2022 04:27:12 GMT
# ARGS: VAULT_VERSION=1.11.3
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 07 Oct 2022 04:27:20 GMT
# ARGS: VAULT_VERSION=1.11.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 07 Oct 2022 04:27:21 GMT
# ARGS: VAULT_VERSION=1.11.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 07 Oct 2022 04:27:21 GMT
VOLUME [/vault/logs]
# Fri, 07 Oct 2022 04:27:22 GMT
VOLUME [/vault/file]
# Fri, 07 Oct 2022 04:27:22 GMT
EXPOSE 8200
# Fri, 07 Oct 2022 04:27:22 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 07 Oct 2022 04:27:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 04:27:22 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33abb1f4412ecd617c25a888039e5e95e9591e4477a535bdf4eb9f639a0a03c6`  
		Last Modified: Fri, 07 Oct 2022 04:28:12 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fccdaef23ddba75b8b22e8df726571a4887aea1eca291fc60ca0464e7504ca9`  
		Last Modified: Fri, 07 Oct 2022 04:28:22 GMT  
		Size: 74.7 MB (74735969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e018fbf02db00931d824e80d70381413695ff777c20d8270acfb156e28d45e57`  
		Last Modified: Fri, 07 Oct 2022 04:28:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb84ed27959e103f1bfb81362c25b5472fe796cc66ff99a777b68d583298358`  
		Last Modified: Fri, 07 Oct 2022 04:28:13 GMT  
		Size: 1.8 KB (1816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:f30429e9665d0b870af7613514b22d09eb8e3312c3a769b994c02e0f5ba71470
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70297307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06c4fd3ece3522b64385b01c48ce3cfbb24327af74b6048a23987ea1094d8324`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:35 GMT
ADD file:8ff80989f06f5a8ffe16c56e00538928dcb1e46faa2b58ab9c14c7227a6cd8f9 in / 
# Tue, 09 Aug 2022 17:49:35 GMT
CMD ["/bin/sh"]
# Wed, 31 Aug 2022 21:49:43 GMT
ARG VAULT_VERSION=1.11.3
# Wed, 31 Aug 2022 21:49:44 GMT
# ARGS: VAULT_VERSION=1.11.3
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 31 Aug 2022 21:49:55 GMT
# ARGS: VAULT_VERSION=1.11.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 31 Aug 2022 21:49:56 GMT
# ARGS: VAULT_VERSION=1.11.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 31 Aug 2022 21:49:56 GMT
VOLUME [/vault/logs]
# Wed, 31 Aug 2022 21:49:56 GMT
VOLUME [/vault/file]
# Wed, 31 Aug 2022 21:49:56 GMT
EXPOSE 8200
# Wed, 31 Aug 2022 21:49:57 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 31 Aug 2022 21:49:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Aug 2022 21:49:57 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:7d147289082e6aa6ef510c09d7c0ac8b5026e0b591f1bfcaf01ceada43c9ec65`  
		Last Modified: Tue, 09 Aug 2022 17:51:04 GMT  
		Size: 2.6 MB (2635498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914e9b4e0991feb43a7b6f4386db37552134233dba7d7e67509e026532e3fc78`  
		Last Modified: Wed, 31 Aug 2022 21:50:50 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191451985f0bf67d8569b41d9eff27bcb25554427eae1c47670635c691828043`  
		Last Modified: Wed, 31 Aug 2022 21:50:59 GMT  
		Size: 67.7 MB (67658537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3e767244b4a31c1ffa01bef811242d0067e732938c98d6b2b73fe55aa3857c`  
		Last Modified: Wed, 31 Aug 2022 21:50:50 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc3cf4938d7600d2fb9408f0b8c6a7b5521f89393695eaf7e8aad62dcc8fbb1`  
		Last Modified: Wed, 31 Aug 2022 21:50:50 GMT  
		Size: 1.8 KB (1816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:7f067bb99986c4f0b7449ff9002f1456900f3c3dc5211939d0fc20a6b8287049
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72347537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7847c948d0303e222e446d85168c3b8b31fbf268f0efa3b3875998fefbff994`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:59 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Tue, 09 Aug 2022 17:39:59 GMT
CMD ["/bin/sh"]
# Wed, 31 Aug 2022 21:47:00 GMT
ARG VAULT_VERSION=1.11.3
# Wed, 31 Aug 2022 21:47:01 GMT
# ARGS: VAULT_VERSION=1.11.3
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 31 Aug 2022 21:47:10 GMT
# ARGS: VAULT_VERSION=1.11.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 31 Aug 2022 21:47:10 GMT
# ARGS: VAULT_VERSION=1.11.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 31 Aug 2022 21:47:11 GMT
VOLUME [/vault/logs]
# Wed, 31 Aug 2022 21:47:12 GMT
VOLUME [/vault/file]
# Wed, 31 Aug 2022 21:47:13 GMT
EXPOSE 8200
# Wed, 31 Aug 2022 21:47:15 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 31 Aug 2022 21:47:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Aug 2022 21:47:16 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef99c9689f07239e0f31a674f13b44e6c80a58182364a3e63c8b1c2af076def1`  
		Last Modified: Wed, 31 Aug 2022 21:48:24 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa2627c8cbee16d9c343f5e884d1e030a26236180d214ca357c13f97c036386`  
		Last Modified: Wed, 31 Aug 2022 21:48:33 GMT  
		Size: 69.6 MB (69622173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45314dd300cb3b4ff0a157e3c3053fd52106832568455081a8b37353c75aea5`  
		Last Modified: Wed, 31 Aug 2022 21:48:24 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08ff4ca234e6c92871957ff044a4a8351918e7f06b609334b4caed4528745a2`  
		Last Modified: Wed, 31 Aug 2022 21:48:24 GMT  
		Size: 1.8 KB (1818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:1b34b6fda393d8a334c4eedc0b175131fc942884cdcca602dd43aaf5837fb797
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73616298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99a14805e808dea6ba008321458115e9beb278026cdc686886e13ca32edc87fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:54 GMT
ADD file:fea8a3ba06779852956b0d3a2dd7514ab33217b1fd395231864c443797f077f6 in / 
# Tue, 09 Aug 2022 17:38:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 02:16:39 GMT
ARG VAULT_VERSION=1.11.3
# Fri, 07 Oct 2022 02:16:40 GMT
# ARGS: VAULT_VERSION=1.11.3
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 07 Oct 2022 02:16:49 GMT
# ARGS: VAULT_VERSION=1.11.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 07 Oct 2022 02:16:50 GMT
# ARGS: VAULT_VERSION=1.11.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 07 Oct 2022 02:16:51 GMT
VOLUME [/vault/logs]
# Fri, 07 Oct 2022 02:16:52 GMT
VOLUME [/vault/file]
# Fri, 07 Oct 2022 02:16:53 GMT
EXPOSE 8200
# Fri, 07 Oct 2022 02:16:55 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 07 Oct 2022 02:16:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 02:16:56 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:2c44f983a875883421e7d5bc471f6437e0e377e6e7343b52c856caee71064d31`  
		Last Modified: Tue, 09 Aug 2022 17:40:01 GMT  
		Size: 2.8 MB (2832612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b10cbdcb59e9628ceffee1669ab783814ef5732d48fd26a88e0b81b3ebb76f`  
		Last Modified: Fri, 07 Oct 2022 02:18:23 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0021f9d2571bc9ba83476d8a0d830aee98a1b7700bc85711a8952951e9c37503`  
		Last Modified: Fri, 07 Oct 2022 02:18:30 GMT  
		Size: 70.8 MB (70780476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a9c4b0a196d9edaa84d26b358a70533e825c3f077842d4b303817245815f20c`  
		Last Modified: Fri, 07 Oct 2022 02:18:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99cb0f64666b4642358204e21488ada2f7edad88fc7f9bf08a3b09be324e9ef2`  
		Last Modified: Fri, 07 Oct 2022 02:18:23 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
