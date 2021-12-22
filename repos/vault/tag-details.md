<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:1.6.7`](#vault167)
-	[`vault:1.7.8`](#vault178)
-	[`vault:1.8.7`](#vault187)
-	[`vault:1.9.2`](#vault192)
-	[`vault:latest`](#vaultlatest)

## `vault:1.6.7`

```console
$ docker pull vault@sha256:dcfe67d671880c5153f6ab135ec36a3ab98a3f412c890eb551b1443e5b18da9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.6.7` - linux; amd64

```console
$ docker pull vault@sha256:769e4cdeeb80e60b64be43783670b59eca416e42c9c5cb184e9d1b505c70dd8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69121489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:becb85347e6688c9bc15931bdf41748d9d12109b8c0ead7e29289ff0a09c45a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:12:51 GMT
ARG VAULT_VERSION=1.6.7
# Sat, 13 Nov 2021 11:12:52 GMT
# ARGS: VAULT_VERSION=1.6.7
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 13 Nov 2021 11:12:59 GMT
# ARGS: VAULT_VERSION=1.6.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 13 Nov 2021 11:13:00 GMT
# ARGS: VAULT_VERSION=1.6.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 13 Nov 2021 11:13:00 GMT
VOLUME [/vault/logs]
# Sat, 13 Nov 2021 11:13:00 GMT
VOLUME [/vault/file]
# Sat, 13 Nov 2021 11:13:01 GMT
EXPOSE 8200
# Sat, 13 Nov 2021 11:13:01 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Nov 2021 11:13:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 11:13:01 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afaffc7ab46f2e497d3fb4e21a99a803da7d654be027e36819fa6f6c1c9e68fb`  
		Last Modified: Sat, 13 Nov 2021 11:14:19 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d934042901383baf557fcb244d4883cacb82e94e53e22071768422a6181192b`  
		Last Modified: Sat, 13 Nov 2021 11:14:28 GMT  
		Size: 66.3 MB (66295235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b98d7be0c6c8866d70de848c0e68b133ccd24844a508c5c0a79c9105a7b2337`  
		Last Modified: Sat, 13 Nov 2021 11:14:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24fafcbd97f1dab71c56fd8e24b30e816d46d3d3202b64b9f977fea9c88978b`  
		Last Modified: Sat, 13 Nov 2021 11:14:19 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.6.7` - linux; arm variant v6

```console
$ docker pull vault@sha256:524d99d3f73246fb85d3956ffdaf38c9ac8849dc4fa0ba874738d16dedc33183
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63853498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eee87097f71ffdac45b773de6ddd2aa95dd6b52b1ac0376428ef6b40203a18b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:46:42 GMT
ARG VAULT_VERSION=1.6.7
# Sat, 13 Nov 2021 06:46:46 GMT
# ARGS: VAULT_VERSION=1.6.7
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 13 Nov 2021 06:47:05 GMT
# ARGS: VAULT_VERSION=1.6.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 13 Nov 2021 06:47:10 GMT
# ARGS: VAULT_VERSION=1.6.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 13 Nov 2021 06:47:10 GMT
VOLUME [/vault/logs]
# Sat, 13 Nov 2021 06:47:12 GMT
VOLUME [/vault/file]
# Sat, 13 Nov 2021 06:47:13 GMT
EXPOSE 8200
# Sat, 13 Nov 2021 06:47:14 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Nov 2021 06:47:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:47:15 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf07e0c178c265c14436ade2f994d8bce9a650a2b903083fd332697ada637be`  
		Last Modified: Sat, 13 Nov 2021 06:50:13 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25890671871c62dbcd9511dd45731941a32275c161a9c1a0d9ca57a79f57c22`  
		Last Modified: Sat, 13 Nov 2021 06:50:33 GMT  
		Size: 61.2 MB (61214831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0966e2693f83897cd8eae486972ef1437b6d73e7c7482b9f2e8e6dfccee197`  
		Last Modified: Sat, 13 Nov 2021 06:50:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f49a35b52f2c6bf2170c927ae58b3266d8b8b5b51fbd26970c0d841b3262f39`  
		Last Modified: Sat, 13 Nov 2021 06:50:13 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.6.7` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:8840b7d40be013e9cdab9d2d3fd7be773c393b7fc54d9397b31685079acb82f9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.1 MB (65140796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33d1a77203679f54ddf4caeae615c322f45566c862584011b5cadf9a71440381`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:13:56 GMT
ARG VAULT_VERSION=1.6.7
# Fri, 12 Nov 2021 18:13:57 GMT
# ARGS: VAULT_VERSION=1.6.7
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 12 Nov 2021 18:14:06 GMT
# ARGS: VAULT_VERSION=1.6.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 12 Nov 2021 18:14:06 GMT
# ARGS: VAULT_VERSION=1.6.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 12 Nov 2021 18:14:07 GMT
VOLUME [/vault/logs]
# Fri, 12 Nov 2021 18:14:08 GMT
VOLUME [/vault/file]
# Fri, 12 Nov 2021 18:14:09 GMT
EXPOSE 8200
# Fri, 12 Nov 2021 18:14:11 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 12 Nov 2021 18:14:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 18:14:12 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3935f9db61a7b34b1919b3b80256bba49848c270324a2bd588211470b1dff16e`  
		Last Modified: Fri, 12 Nov 2021 18:15:45 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8dff2b8919eb42c25188a65f6e57a79078ba59cd83d05523de7da486c63a194`  
		Last Modified: Fri, 12 Nov 2021 18:15:54 GMT  
		Size: 62.4 MB (62419882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2280cedd357aedae89538f83f73221c1532723e29e2b1238ea78213a11f5797`  
		Last Modified: Fri, 12 Nov 2021 18:15:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c647a93f11944fbcdebdbd789ed54da45d27b7bfe5d5b610986a0e5800a9dc18`  
		Last Modified: Fri, 12 Nov 2021 18:15:45 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.6.7` - linux; 386

```console
$ docker pull vault@sha256:967f16406d097d62460fbc18b68cb72d2a722ae1a772b97ee851af7970662ba7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67164972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f64270dc212452748714f3e270f2e08ed6fdaef36b141351bc4a050fa213460`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 17:32:53 GMT
ARG VAULT_VERSION=1.6.7
# Fri, 12 Nov 2021 17:32:54 GMT
# ARGS: VAULT_VERSION=1.6.7
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 12 Nov 2021 17:33:11 GMT
# ARGS: VAULT_VERSION=1.6.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 12 Nov 2021 17:33:13 GMT
# ARGS: VAULT_VERSION=1.6.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 12 Nov 2021 17:33:13 GMT
VOLUME [/vault/logs]
# Fri, 12 Nov 2021 17:33:14 GMT
VOLUME [/vault/file]
# Fri, 12 Nov 2021 17:33:14 GMT
EXPOSE 8200
# Fri, 12 Nov 2021 17:33:14 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 12 Nov 2021 17:33:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 17:33:15 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5687af1e758a81cb56968feabeb4df42f60ba6f22267571b48e04f30c8b669`  
		Last Modified: Fri, 12 Nov 2021 17:35:38 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6d591c10a0632df92caf56171ceda32aea7eaf3cf2605bbb78b4958e868552`  
		Last Modified: Fri, 12 Nov 2021 17:35:53 GMT  
		Size: 64.3 MB (64330751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926a723f3932c401b81e4a0896005dd52ff449a3fcd29f2ca4b10d842f48d9c2`  
		Last Modified: Fri, 12 Nov 2021 17:35:38 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280f02b1aec09a9f6bba587e771bafcad59c851053c9f0fa1963b5d0413dc981`  
		Last Modified: Fri, 12 Nov 2021 17:35:38 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.7.8`

```console
$ docker pull vault@sha256:115dbaf4c108b0f55bf71157c4924f604e691dc7c5b51a2b01f55a78da7a71ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.7.8` - linux; amd64

```console
$ docker pull vault@sha256:16c6be4921e109f5270374572c8f088cff8ddd57cb32654cdbdd1a55bcb406db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68128201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fd104f49d5b01245d876ac84bcf1ffc0b1f2aedcc2eff2a0e5a28db82dfce7f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 22 Dec 2021 22:03:16 GMT
ARG VAULT_VERSION=1.7.8
# Wed, 22 Dec 2021 22:03:17 GMT
# ARGS: VAULT_VERSION=1.7.8
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Dec 2021 22:03:24 GMT
# ARGS: VAULT_VERSION=1.7.8
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Dec 2021 22:03:25 GMT
# ARGS: VAULT_VERSION=1.7.8
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Dec 2021 22:03:25 GMT
VOLUME [/vault/logs]
# Wed, 22 Dec 2021 22:03:25 GMT
VOLUME [/vault/file]
# Wed, 22 Dec 2021 22:03:25 GMT
EXPOSE 8200
# Wed, 22 Dec 2021 22:03:26 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Dec 2021 22:03:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Dec 2021 22:03:26 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8b90e0180da1fd6b47704b969e09de029b8873619144779bb1bacd6cac5a3d`  
		Last Modified: Wed, 22 Dec 2021 22:04:15 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa0b6bd4f051e984fbe2c349d7dbb4d4d73b160b6931625b746302a4f43ab75`  
		Last Modified: Wed, 22 Dec 2021 22:04:25 GMT  
		Size: 65.3 MB (65301943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb42e4f97c363a06e9b329b04e825d1581124a2459fcc56a55c5dc791a92bc7`  
		Last Modified: Wed, 22 Dec 2021 22:04:15 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e813e8752670ff562dfda12e729206d8d658082d532463c5d1366bb763c84c5e`  
		Last Modified: Wed, 22 Dec 2021 22:04:15 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.7.8` - linux; arm variant v6

```console
$ docker pull vault@sha256:69a3805cbf808c9aa2b8d60b6417a93173a2a5157b487e48421d2c44f7a762a9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.9 MB (62870632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca7ef1e3aadefd6516e5c8c2a8da223d4ae170bb00013025514dc3521423c9b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Wed, 22 Dec 2021 18:53:31 GMT
ARG VAULT_VERSION=1.7.8
# Wed, 22 Dec 2021 18:53:33 GMT
# ARGS: VAULT_VERSION=1.7.8
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Dec 2021 18:53:54 GMT
# ARGS: VAULT_VERSION=1.7.8
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Dec 2021 18:53:56 GMT
# ARGS: VAULT_VERSION=1.7.8
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Dec 2021 18:53:57 GMT
VOLUME [/vault/logs]
# Wed, 22 Dec 2021 18:53:57 GMT
VOLUME [/vault/file]
# Wed, 22 Dec 2021 18:53:57 GMT
EXPOSE 8200
# Wed, 22 Dec 2021 18:53:58 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Dec 2021 18:53:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Dec 2021 18:53:59 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0adcb6de320f9bbc16e1483ee9b57f4a15476beff0cb4c9183e1936d297044`  
		Last Modified: Wed, 22 Dec 2021 18:56:01 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78359d04791c737043581aadd1464e81403b2502d5e8c31b66f0c49f2486b2a4`  
		Last Modified: Wed, 22 Dec 2021 18:56:31 GMT  
		Size: 60.2 MB (60231961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab1b9250e548a667000b23c12f5e96ce6f7eb389e78e3a911c3aa530af27f81`  
		Last Modified: Wed, 22 Dec 2021 18:56:01 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0255ce4cf462c28cbadc00e5fbcb60e3380a343f070e5b7de01f78e69e212381`  
		Last Modified: Wed, 22 Dec 2021 18:56:01 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.7.8` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:ab7f4f7bc837ecb423358335b606e5a2fa720d264fa6d8e04ef6322b34ce5745
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.5 MB (64527034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9ffda4394775789783851eeda4e0c1d25ed8bea593a2455ceb271d53406f26b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Wed, 22 Dec 2021 20:34:24 GMT
ARG VAULT_VERSION=1.7.8
# Wed, 22 Dec 2021 20:34:25 GMT
# ARGS: VAULT_VERSION=1.7.8
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Dec 2021 20:34:37 GMT
# ARGS: VAULT_VERSION=1.7.8
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Dec 2021 20:34:38 GMT
# ARGS: VAULT_VERSION=1.7.8
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Dec 2021 20:34:39 GMT
VOLUME [/vault/logs]
# Wed, 22 Dec 2021 20:34:40 GMT
VOLUME [/vault/file]
# Wed, 22 Dec 2021 20:34:41 GMT
EXPOSE 8200
# Wed, 22 Dec 2021 20:34:43 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Dec 2021 20:34:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Dec 2021 20:34:44 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0044ac6eccfaf1b3db4cf66c34d27dd52f1750c2bfbf621fcdb9e0127384b98e`  
		Last Modified: Wed, 22 Dec 2021 20:36:46 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5674497e6b29d80c411a410107f4c01c6d076b35482e10000d060a863c7a5aaa`  
		Last Modified: Wed, 22 Dec 2021 20:36:54 GMT  
		Size: 61.8 MB (61806118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e27da8d43366b473042286b8baaee2a5b9960d968ff0b941d56322d8369a462`  
		Last Modified: Wed, 22 Dec 2021 20:36:46 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ccbd4eb781945dacf156a64da92c65ba9782d0356f2d10b1c29ef4e13ad6c80`  
		Last Modified: Wed, 22 Dec 2021 20:36:46 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.7.8` - linux; 386

```console
$ docker pull vault@sha256:b798dd92041207eabc5752880f42719895e9feb7ce7b407061ffd6ceffc14f7f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (66001814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbb72d5e902e499445c970f69ad5af1cd6a5841375fdf4ec703d9f704f046ba3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Wed, 22 Dec 2021 20:52:07 GMT
ARG VAULT_VERSION=1.7.8
# Wed, 22 Dec 2021 20:52:08 GMT
# ARGS: VAULT_VERSION=1.7.8
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Dec 2021 20:52:22 GMT
# ARGS: VAULT_VERSION=1.7.8
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Dec 2021 20:52:24 GMT
# ARGS: VAULT_VERSION=1.7.8
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Dec 2021 20:52:24 GMT
VOLUME [/vault/logs]
# Wed, 22 Dec 2021 20:52:25 GMT
VOLUME [/vault/file]
# Wed, 22 Dec 2021 20:52:25 GMT
EXPOSE 8200
# Wed, 22 Dec 2021 20:52:25 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Dec 2021 20:52:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Dec 2021 20:52:26 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fc15a6595c93d764ebaad78f4bb1386988302226c67f13d9ed8e163f648b7e`  
		Last Modified: Wed, 22 Dec 2021 20:53:44 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5fde30e47614764e482e083920dad0c841f28054cad19835d84922375c368b5`  
		Last Modified: Wed, 22 Dec 2021 20:53:58 GMT  
		Size: 63.2 MB (63167584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a01d585213cf39b8b642d7b14640d31308861efade390babdb8eaaa98aeb8ff`  
		Last Modified: Wed, 22 Dec 2021 20:53:44 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d04dfe73fec36f7707897c62b34fd72752248ebd76498657aa8905c610b4a1d`  
		Last Modified: Wed, 22 Dec 2021 20:53:44 GMT  
		Size: 1.8 KB (1826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.8.7`

```console
$ docker pull vault@sha256:e7105050b40095848dc5f56afc6b60dcdf9cd7ed3fbea9532707ed2052d2906c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.8.7` - linux; amd64

```console
$ docker pull vault@sha256:94574a967ad25c754067df94f7cd237057d3ef6ab1be4c0a5aff91b5180ec5b7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70575894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e065ea61c87b552a22ab8c8d1dacef0e40c7c1de903e6e4abf0082d93c1f8d1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 22 Dec 2021 22:03:03 GMT
ARG VAULT_VERSION=1.8.7
# Wed, 22 Dec 2021 22:03:03 GMT
# ARGS: VAULT_VERSION=1.8.7
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Dec 2021 22:03:11 GMT
# ARGS: VAULT_VERSION=1.8.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Dec 2021 22:03:12 GMT
# ARGS: VAULT_VERSION=1.8.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Dec 2021 22:03:12 GMT
VOLUME [/vault/logs]
# Wed, 22 Dec 2021 22:03:13 GMT
VOLUME [/vault/file]
# Wed, 22 Dec 2021 22:03:13 GMT
EXPOSE 8200
# Wed, 22 Dec 2021 22:03:13 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Dec 2021 22:03:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Dec 2021 22:03:13 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7273410f6472d26596577b403eb781f0f5e6f6bf0dac69a2706d0563a61b1900`  
		Last Modified: Wed, 22 Dec 2021 22:03:57 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:854cd52f8ddb92ac93818f4b9f7d1867d9eb4ac7f6bdf1d79f04ec76555739f0`  
		Last Modified: Wed, 22 Dec 2021 22:04:06 GMT  
		Size: 67.7 MB (67749632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0af89158e0dc724661cbc33e53877bd70e99dcc4666224cf9811ac180a8f682`  
		Last Modified: Wed, 22 Dec 2021 22:03:58 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf6f2e41e972ceaeff29eb5a5e93aef67a9d223469f3438a6c194b52cd1e72b`  
		Last Modified: Wed, 22 Dec 2021 22:03:57 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.8.7` - linux; arm variant v6

```console
$ docker pull vault@sha256:d06188ed1cc33531d8e87b260c6e807522920673b8742474f440a8ab25d06d6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64945329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:374d09249f327b0e4e5fac6998bbbb78ef7fa1ee35293aa18dd2e6621ab7595b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Wed, 22 Dec 2021 18:52:52 GMT
ARG VAULT_VERSION=1.8.7
# Wed, 22 Dec 2021 18:52:54 GMT
# ARGS: VAULT_VERSION=1.8.7
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Dec 2021 18:53:16 GMT
# ARGS: VAULT_VERSION=1.8.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Dec 2021 18:53:18 GMT
# ARGS: VAULT_VERSION=1.8.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Dec 2021 18:53:19 GMT
VOLUME [/vault/logs]
# Wed, 22 Dec 2021 18:53:19 GMT
VOLUME [/vault/file]
# Wed, 22 Dec 2021 18:53:19 GMT
EXPOSE 8200
# Wed, 22 Dec 2021 18:53:20 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Dec 2021 18:53:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Dec 2021 18:53:21 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9f6137f34f978c8aaa242b7b2b4d34b82867aa2ea75c8a2aac2ff07e901c38`  
		Last Modified: Wed, 22 Dec 2021 18:55:23 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ac03000e5fb89485810d5f9c1c6bc67e66a2dc9c37a98311c899f9b7dbb49f`  
		Last Modified: Wed, 22 Dec 2021 18:55:53 GMT  
		Size: 62.3 MB (62306657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751503ece84a110522b2806a652eae62461e994cf882c191a3d6719852cef2c4`  
		Last Modified: Wed, 22 Dec 2021 18:55:23 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7130722044028a7bb4a8520667a2af0b439b34fbf020b1b5b9168d9cc790f6ca`  
		Last Modified: Wed, 22 Dec 2021 18:55:23 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.8.7` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:e49f25c7c472bb4eada7643322306e58a11385babf1923785dd521d2e445b7c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66858002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6128d1ea90cad1311347f681243d712ceb9ecfad696e2e409182cf22cc45b792`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Wed, 22 Dec 2021 20:33:57 GMT
ARG VAULT_VERSION=1.8.7
# Wed, 22 Dec 2021 20:33:58 GMT
# ARGS: VAULT_VERSION=1.8.7
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Dec 2021 20:34:13 GMT
# ARGS: VAULT_VERSION=1.8.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Dec 2021 20:34:14 GMT
# ARGS: VAULT_VERSION=1.8.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Dec 2021 20:34:14 GMT
VOLUME [/vault/logs]
# Wed, 22 Dec 2021 20:34:15 GMT
VOLUME [/vault/file]
# Wed, 22 Dec 2021 20:34:16 GMT
EXPOSE 8200
# Wed, 22 Dec 2021 20:34:18 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Dec 2021 20:34:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Dec 2021 20:34:19 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8912665e4bb4e4482945f88bc8fa4ac9cb4f6cbb9da48845f1ca9d63c2aec7f3`  
		Last Modified: Wed, 22 Dec 2021 20:36:30 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330d6de436adc47da472462abfa58b02245857f880aa74513e485f8aa8638044`  
		Last Modified: Wed, 22 Dec 2021 20:36:38 GMT  
		Size: 64.1 MB (64137087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8a214e07a5750854e83103bc150b1fe20f9bf9a9481605aed307bf90968164`  
		Last Modified: Wed, 22 Dec 2021 20:36:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62882909818c38456bc32148d0ce76258d8b3a3fca1eb2999f2e467139ec6ff`  
		Last Modified: Wed, 22 Dec 2021 20:36:30 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.8.7` - linux; 386

```console
$ docker pull vault@sha256:045b142d694f14097491689ebe9fc9d4d8ae5424a8e629c409180a5dd8551ac3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68309411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:333c766adf225a75333eca687c3f203165c6717ba165367e37c13c4c76e06acb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Wed, 22 Dec 2021 20:51:38 GMT
ARG VAULT_VERSION=1.8.7
# Wed, 22 Dec 2021 20:51:40 GMT
# ARGS: VAULT_VERSION=1.8.7
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Dec 2021 20:51:56 GMT
# ARGS: VAULT_VERSION=1.8.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Dec 2021 20:51:58 GMT
# ARGS: VAULT_VERSION=1.8.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Dec 2021 20:51:59 GMT
VOLUME [/vault/logs]
# Wed, 22 Dec 2021 20:51:59 GMT
VOLUME [/vault/file]
# Wed, 22 Dec 2021 20:51:59 GMT
EXPOSE 8200
# Wed, 22 Dec 2021 20:51:59 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Dec 2021 20:52:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Dec 2021 20:52:00 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0f7a64ae125d960cd39b49fb91ac79bb031b64e1c85206fd293a7b813ec1d3`  
		Last Modified: Wed, 22 Dec 2021 20:53:21 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123e37e56ba3d82671892a261d1c3def5d21dcfee94d4daec24c43f3d6e1dc40`  
		Last Modified: Wed, 22 Dec 2021 20:53:35 GMT  
		Size: 65.5 MB (65475188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f193570b3e6930396558eeb3db90aee3bd07f86e9ac1178cd264aa90524ecef9`  
		Last Modified: Wed, 22 Dec 2021 20:53:21 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da4e1f2189cb3285a921bc038702dda01824358b08bbfba21a61dd49a5faee0`  
		Last Modified: Wed, 22 Dec 2021 20:53:21 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.9.2`

```console
$ docker pull vault@sha256:cc7bca14ebe2e6f32401bf5e59c1b95081c387b75fb0c06c18c085670338a59b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.9.2` - linux; amd64

```console
$ docker pull vault@sha256:120f43bbc0ee041245631b78e6287e93861ae73674c034e4882bdc30290cf638
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72932445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bb605f7fffed3a5db4aaa27c80eb0c9b5de898356ebf5e66c7897fce56f29f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 22 Dec 2021 22:02:49 GMT
ARG VAULT_VERSION=1.9.2
# Wed, 22 Dec 2021 22:02:50 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Dec 2021 22:02:58 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Dec 2021 22:02:59 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Dec 2021 22:02:59 GMT
VOLUME [/vault/logs]
# Wed, 22 Dec 2021 22:02:59 GMT
VOLUME [/vault/file]
# Wed, 22 Dec 2021 22:03:00 GMT
EXPOSE 8200
# Wed, 22 Dec 2021 22:03:00 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Dec 2021 22:03:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Dec 2021 22:03:00 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250eba83471e864023d238d7abbb96696bda8bda36f593f865b2aba942906be5`  
		Last Modified: Wed, 22 Dec 2021 22:03:39 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0778ed8dc3c55ba6c08cdb43c8de991ab5aedaa82eaad0489d1f2df7275223`  
		Last Modified: Wed, 22 Dec 2021 22:03:48 GMT  
		Size: 70.1 MB (70106184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04235f19b893279594f8e24d437da5a44d33c0631925aabad650223253f7c302`  
		Last Modified: Wed, 22 Dec 2021 22:03:39 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4279ec1af0bf74afd5930fccefe77382fecb716f683ca466e18184fd8b2971`  
		Last Modified: Wed, 22 Dec 2021 22:03:39 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.9.2` - linux; arm variant v6

```console
$ docker pull vault@sha256:76b197761a6bf77dfb6940f47db781306b0e4a99bfe395ca4669ff664bbb5291
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66295841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1ba640002891c65168c01e7a6e1b8cec7febed127e265b4379ef85cbc7c9916`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Wed, 22 Dec 2021 18:52:08 GMT
ARG VAULT_VERSION=1.9.2
# Wed, 22 Dec 2021 18:52:10 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Dec 2021 18:52:33 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Dec 2021 18:52:36 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Dec 2021 18:52:36 GMT
VOLUME [/vault/logs]
# Wed, 22 Dec 2021 18:52:37 GMT
VOLUME [/vault/file]
# Wed, 22 Dec 2021 18:52:37 GMT
EXPOSE 8200
# Wed, 22 Dec 2021 18:52:38 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Dec 2021 18:52:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Dec 2021 18:52:39 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5fbd7bbaabf55cbd282ff7af64151efb458e0edee017c68d7bdf7766677e4e`  
		Last Modified: Wed, 22 Dec 2021 18:54:39 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e9009a848717349f1d6242a89736d2b8073aa576394471f6aa24d964989fa3`  
		Last Modified: Wed, 22 Dec 2021 18:55:11 GMT  
		Size: 63.7 MB (63657167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51995fc39f8fc00b85e75f5783bfaf923f5b06eefedadfb2adb76b66abe3777`  
		Last Modified: Wed, 22 Dec 2021 18:54:39 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:021ac818a2ef8ca123fcea90c7a99d831184f6304756725821e2df1dd7f3fc15`  
		Last Modified: Wed, 22 Dec 2021 18:54:38 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.9.2` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:a0a2220c6a23c21de8f2d0e5f77dc9ebc13275b5701c63e29c8e2a5489d993c3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (68037636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8499333f487fe90ab525d89fa43bf90adf8a35faac7ff2310a7c18ad7df3111`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Wed, 22 Dec 2021 20:33:34 GMT
ARG VAULT_VERSION=1.9.2
# Wed, 22 Dec 2021 20:33:35 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Dec 2021 20:33:45 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Dec 2021 20:33:46 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Dec 2021 20:33:47 GMT
VOLUME [/vault/logs]
# Wed, 22 Dec 2021 20:33:48 GMT
VOLUME [/vault/file]
# Wed, 22 Dec 2021 20:33:49 GMT
EXPOSE 8200
# Wed, 22 Dec 2021 20:33:51 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Dec 2021 20:33:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Dec 2021 20:33:52 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29cd82552317e13f3a0054fca119ff706150dda8729d6589efe4c4765d77c21`  
		Last Modified: Wed, 22 Dec 2021 20:36:11 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34d78dbd99bfed725c39afb795ec1fc1cdf594b6ff131c23bb935631608b175`  
		Last Modified: Wed, 22 Dec 2021 20:36:20 GMT  
		Size: 65.3 MB (65316720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a70fd74408902fa7157c49cfb1f48ec79d7f3b7be57e95525275c480ccfe73`  
		Last Modified: Wed, 22 Dec 2021 20:36:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ab137c020ad06a85a7f54d082fd711bcee0e4709847e4c38aa23eeaf241ab56`  
		Last Modified: Wed, 22 Dec 2021 20:36:11 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.9.2` - linux; 386

```console
$ docker pull vault@sha256:4d487e3d65910ec32f0dde45c570113467c73ba52feb45f6a2d2040bf17a6a2a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.3 MB (69318144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a6ad23000600034347b2e05570777e3ed95c69bde23d86ba31abbe87de2299`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Wed, 22 Dec 2021 20:51:01 GMT
ARG VAULT_VERSION=1.9.2
# Wed, 22 Dec 2021 20:51:04 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Dec 2021 20:51:20 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Dec 2021 20:51:23 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Dec 2021 20:51:23 GMT
VOLUME [/vault/logs]
# Wed, 22 Dec 2021 20:51:24 GMT
VOLUME [/vault/file]
# Wed, 22 Dec 2021 20:51:24 GMT
EXPOSE 8200
# Wed, 22 Dec 2021 20:51:25 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Dec 2021 20:51:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Dec 2021 20:51:26 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e32432e839d9410dbf95acf62b3b3ee7c59d82d456fe23ee022cb11b6d56ce`  
		Last Modified: Wed, 22 Dec 2021 20:52:54 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c892bcdaac8c4aff93adfeb21a91b79e178664e79961b1805d5a935272da86f6`  
		Last Modified: Wed, 22 Dec 2021 20:53:08 GMT  
		Size: 66.5 MB (66483915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6252140138ca5729ca2d033d267a3b01ae43ea862d21c5ed66bd2f1b615dc8cf`  
		Last Modified: Wed, 22 Dec 2021 20:52:54 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966e79a98d455d952534442339429acb2459d3aa0d391ee39eff0a361c454d81`  
		Last Modified: Wed, 22 Dec 2021 20:52:54 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:latest`

```console
$ docker pull vault@sha256:cc7bca14ebe2e6f32401bf5e59c1b95081c387b75fb0c06c18c085670338a59b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:120f43bbc0ee041245631b78e6287e93861ae73674c034e4882bdc30290cf638
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72932445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bb605f7fffed3a5db4aaa27c80eb0c9b5de898356ebf5e66c7897fce56f29f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 22 Dec 2021 22:02:49 GMT
ARG VAULT_VERSION=1.9.2
# Wed, 22 Dec 2021 22:02:50 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Dec 2021 22:02:58 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Dec 2021 22:02:59 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Dec 2021 22:02:59 GMT
VOLUME [/vault/logs]
# Wed, 22 Dec 2021 22:02:59 GMT
VOLUME [/vault/file]
# Wed, 22 Dec 2021 22:03:00 GMT
EXPOSE 8200
# Wed, 22 Dec 2021 22:03:00 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Dec 2021 22:03:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Dec 2021 22:03:00 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250eba83471e864023d238d7abbb96696bda8bda36f593f865b2aba942906be5`  
		Last Modified: Wed, 22 Dec 2021 22:03:39 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0778ed8dc3c55ba6c08cdb43c8de991ab5aedaa82eaad0489d1f2df7275223`  
		Last Modified: Wed, 22 Dec 2021 22:03:48 GMT  
		Size: 70.1 MB (70106184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04235f19b893279594f8e24d437da5a44d33c0631925aabad650223253f7c302`  
		Last Modified: Wed, 22 Dec 2021 22:03:39 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4279ec1af0bf74afd5930fccefe77382fecb716f683ca466e18184fd8b2971`  
		Last Modified: Wed, 22 Dec 2021 22:03:39 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:76b197761a6bf77dfb6940f47db781306b0e4a99bfe395ca4669ff664bbb5291
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66295841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1ba640002891c65168c01e7a6e1b8cec7febed127e265b4379ef85cbc7c9916`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Wed, 22 Dec 2021 18:52:08 GMT
ARG VAULT_VERSION=1.9.2
# Wed, 22 Dec 2021 18:52:10 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Dec 2021 18:52:33 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Dec 2021 18:52:36 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Dec 2021 18:52:36 GMT
VOLUME [/vault/logs]
# Wed, 22 Dec 2021 18:52:37 GMT
VOLUME [/vault/file]
# Wed, 22 Dec 2021 18:52:37 GMT
EXPOSE 8200
# Wed, 22 Dec 2021 18:52:38 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Dec 2021 18:52:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Dec 2021 18:52:39 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5fbd7bbaabf55cbd282ff7af64151efb458e0edee017c68d7bdf7766677e4e`  
		Last Modified: Wed, 22 Dec 2021 18:54:39 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e9009a848717349f1d6242a89736d2b8073aa576394471f6aa24d964989fa3`  
		Last Modified: Wed, 22 Dec 2021 18:55:11 GMT  
		Size: 63.7 MB (63657167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51995fc39f8fc00b85e75f5783bfaf923f5b06eefedadfb2adb76b66abe3777`  
		Last Modified: Wed, 22 Dec 2021 18:54:39 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:021ac818a2ef8ca123fcea90c7a99d831184f6304756725821e2df1dd7f3fc15`  
		Last Modified: Wed, 22 Dec 2021 18:54:38 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:a0a2220c6a23c21de8f2d0e5f77dc9ebc13275b5701c63e29c8e2a5489d993c3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (68037636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8499333f487fe90ab525d89fa43bf90adf8a35faac7ff2310a7c18ad7df3111`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Wed, 22 Dec 2021 20:33:34 GMT
ARG VAULT_VERSION=1.9.2
# Wed, 22 Dec 2021 20:33:35 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Dec 2021 20:33:45 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Dec 2021 20:33:46 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Dec 2021 20:33:47 GMT
VOLUME [/vault/logs]
# Wed, 22 Dec 2021 20:33:48 GMT
VOLUME [/vault/file]
# Wed, 22 Dec 2021 20:33:49 GMT
EXPOSE 8200
# Wed, 22 Dec 2021 20:33:51 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Dec 2021 20:33:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Dec 2021 20:33:52 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29cd82552317e13f3a0054fca119ff706150dda8729d6589efe4c4765d77c21`  
		Last Modified: Wed, 22 Dec 2021 20:36:11 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34d78dbd99bfed725c39afb795ec1fc1cdf594b6ff131c23bb935631608b175`  
		Last Modified: Wed, 22 Dec 2021 20:36:20 GMT  
		Size: 65.3 MB (65316720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a70fd74408902fa7157c49cfb1f48ec79d7f3b7be57e95525275c480ccfe73`  
		Last Modified: Wed, 22 Dec 2021 20:36:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ab137c020ad06a85a7f54d082fd711bcee0e4709847e4c38aa23eeaf241ab56`  
		Last Modified: Wed, 22 Dec 2021 20:36:11 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:4d487e3d65910ec32f0dde45c570113467c73ba52feb45f6a2d2040bf17a6a2a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.3 MB (69318144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a6ad23000600034347b2e05570777e3ed95c69bde23d86ba31abbe87de2299`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Wed, 22 Dec 2021 20:51:01 GMT
ARG VAULT_VERSION=1.9.2
# Wed, 22 Dec 2021 20:51:04 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Dec 2021 20:51:20 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Dec 2021 20:51:23 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Dec 2021 20:51:23 GMT
VOLUME [/vault/logs]
# Wed, 22 Dec 2021 20:51:24 GMT
VOLUME [/vault/file]
# Wed, 22 Dec 2021 20:51:24 GMT
EXPOSE 8200
# Wed, 22 Dec 2021 20:51:25 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Dec 2021 20:51:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Dec 2021 20:51:26 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e32432e839d9410dbf95acf62b3b3ee7c59d82d456fe23ee022cb11b6d56ce`  
		Last Modified: Wed, 22 Dec 2021 20:52:54 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c892bcdaac8c4aff93adfeb21a91b79e178664e79961b1805d5a935272da86f6`  
		Last Modified: Wed, 22 Dec 2021 20:53:08 GMT  
		Size: 66.5 MB (66483915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6252140138ca5729ca2d033d267a3b01ae43ea862d21c5ed66bd2f1b615dc8cf`  
		Last Modified: Wed, 22 Dec 2021 20:52:54 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966e79a98d455d952534442339429acb2459d3aa0d391ee39eff0a361c454d81`  
		Last Modified: Wed, 22 Dec 2021 20:52:54 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
