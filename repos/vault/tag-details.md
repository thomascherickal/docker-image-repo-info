<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:1.6.7`](#vault167)
-	[`vault:1.7.9`](#vault179)
-	[`vault:1.8.8`](#vault188)
-	[`vault:1.9.3`](#vault193)
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

## `vault:1.7.9`

```console
$ docker pull vault@sha256:704c89314f54152c22588ff8784351d799a3bbfcde70fb91e7f6eace10d96c4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `vault:1.7.9` - linux; arm variant v6

```console
$ docker pull vault@sha256:a3fc0aa4853c37de3e3e4f94c2fe64cf21fbc336d8619c428336d8dcf8a9f0e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.9 MB (62861139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:860901407465683f35e4b6fab1251e7f58464a1d305f800504350ca94a69a4a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 29 Jan 2022 04:05:38 GMT
ARG VAULT_VERSION=1.7.9
# Sat, 29 Jan 2022 04:05:40 GMT
# ARGS: VAULT_VERSION=1.7.9
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 29 Jan 2022 04:06:05 GMT
# ARGS: VAULT_VERSION=1.7.9
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 29 Jan 2022 04:06:07 GMT
# ARGS: VAULT_VERSION=1.7.9
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 29 Jan 2022 04:06:08 GMT
VOLUME [/vault/logs]
# Sat, 29 Jan 2022 04:06:08 GMT
VOLUME [/vault/file]
# Sat, 29 Jan 2022 04:06:09 GMT
EXPOSE 8200
# Sat, 29 Jan 2022 04:06:09 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 29 Jan 2022 04:06:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 29 Jan 2022 04:06:10 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca20ada8e1f9a50507402b2e94058cf950ff34c51bb9d07c7db2e238d7b5b761`  
		Last Modified: Sat, 29 Jan 2022 04:08:21 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033e35df1423c72f4fd04c43ce8c2dc965d5fdcbbbacd719584b4d15aff16101`  
		Last Modified: Sat, 29 Jan 2022 04:08:52 GMT  
		Size: 60.2 MB (60222469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79cb755edd1c28eeb1a8531aa62059c9001ff5b3a7e5be4884475dfa46c983bf`  
		Last Modified: Sat, 29 Jan 2022 04:08:21 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc754759898f58e9036656ed1516ccddd953e733a81159e5f317c96be755cf2`  
		Last Modified: Sat, 29 Jan 2022 04:08:21 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.8.8`

```console
$ docker pull vault@sha256:e2dd9103c774623e4d274413682bd4b0c16a13217081af67919a3de10ce60778
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `vault:1.8.8` - linux; arm variant v6

```console
$ docker pull vault@sha256:a60f548f8d74dde6956258e3bf28e76259ddc313948f8006dd80b5f2d88e61fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (64950462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:359484fe50e0340c52b4c1f8d5eb1a4da53db3616b2f2f218577bdc62fc50709`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 29 Jan 2022 04:04:55 GMT
ARG VAULT_VERSION=1.8.8
# Sat, 29 Jan 2022 04:04:57 GMT
# ARGS: VAULT_VERSION=1.8.8
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 29 Jan 2022 04:05:23 GMT
# ARGS: VAULT_VERSION=1.8.8
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 29 Jan 2022 04:05:25 GMT
# ARGS: VAULT_VERSION=1.8.8
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 29 Jan 2022 04:05:25 GMT
VOLUME [/vault/logs]
# Sat, 29 Jan 2022 04:05:26 GMT
VOLUME [/vault/file]
# Sat, 29 Jan 2022 04:05:26 GMT
EXPOSE 8200
# Sat, 29 Jan 2022 04:05:27 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 29 Jan 2022 04:05:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 29 Jan 2022 04:05:28 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350dfaad1e33ba4428d576221af393bdd5aaaf7d24301036aaa12a6a07b80c71`  
		Last Modified: Sat, 29 Jan 2022 04:07:38 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bafb83c9543429e9124789993f0f76bd75d69e957e90c3098c3924b3e0a9041b`  
		Last Modified: Sat, 29 Jan 2022 04:08:11 GMT  
		Size: 62.3 MB (62311791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae3a0f27aee14cd181ce5b1e590c344c4fda31fa76fe81b0e44e518420529b8`  
		Last Modified: Sat, 29 Jan 2022 04:07:38 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a523bdf7b76555c60de97431714dfbdfc9cd162ebec690c9d4ea54ef23913360`  
		Last Modified: Sat, 29 Jan 2022 04:07:38 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.9.3`

```console
$ docker pull vault@sha256:5fb319ea228b7e1b5ae94b425abfbe94d2202c1f81a8d8ba8fef1958e5a20190
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `vault:1.9.3` - linux; arm variant v6

```console
$ docker pull vault@sha256:2babf0270263c3200f55f9bc64497dcc29ec3dfd097e0cab21831f7ffb00f8f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66292967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a64a1295c0eac5a9a29d1d7dee6e8f7ff583a1c11bc00aa671bf316ef7628b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 29 Jan 2022 04:04:03 GMT
ARG VAULT_VERSION=1.9.3
# Sat, 29 Jan 2022 04:04:05 GMT
# ARGS: VAULT_VERSION=1.9.3
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 29 Jan 2022 04:04:39 GMT
# ARGS: VAULT_VERSION=1.9.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 29 Jan 2022 04:04:41 GMT
# ARGS: VAULT_VERSION=1.9.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 29 Jan 2022 04:04:41 GMT
VOLUME [/vault/logs]
# Sat, 29 Jan 2022 04:04:42 GMT
VOLUME [/vault/file]
# Sat, 29 Jan 2022 04:04:42 GMT
EXPOSE 8200
# Sat, 29 Jan 2022 04:04:43 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 29 Jan 2022 04:04:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 29 Jan 2022 04:04:44 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade36def3541e42ce15ffd1bf5ea1cc250cceb84a44de9f9d146e01deece7c4b`  
		Last Modified: Sat, 29 Jan 2022 04:06:52 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256b385799d95f1efdf26f2bc43addfdf0065556663579e9ff14558374cfc5e6`  
		Last Modified: Sat, 29 Jan 2022 04:07:26 GMT  
		Size: 63.7 MB (63654296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca46c14046a0a310dccae103438982827ebf0d5e184fc2958966363786623bd`  
		Last Modified: Sat, 29 Jan 2022 04:06:52 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acbbd623f5ce9237f9a46d32a7cd7651ebb72a38d2024e2000b7ab0909d1611`  
		Last Modified: Sat, 29 Jan 2022 04:06:52 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:latest`

```console
$ docker pull vault@sha256:4b1855757d2050d026e7d016ec77b76d5ece8140d1a0b974e4adb36ba54134c4
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
$ docker pull vault@sha256:2babf0270263c3200f55f9bc64497dcc29ec3dfd097e0cab21831f7ffb00f8f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66292967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a64a1295c0eac5a9a29d1d7dee6e8f7ff583a1c11bc00aa671bf316ef7628b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 29 Jan 2022 04:04:03 GMT
ARG VAULT_VERSION=1.9.3
# Sat, 29 Jan 2022 04:04:05 GMT
# ARGS: VAULT_VERSION=1.9.3
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 29 Jan 2022 04:04:39 GMT
# ARGS: VAULT_VERSION=1.9.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 29 Jan 2022 04:04:41 GMT
# ARGS: VAULT_VERSION=1.9.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 29 Jan 2022 04:04:41 GMT
VOLUME [/vault/logs]
# Sat, 29 Jan 2022 04:04:42 GMT
VOLUME [/vault/file]
# Sat, 29 Jan 2022 04:04:42 GMT
EXPOSE 8200
# Sat, 29 Jan 2022 04:04:43 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 29 Jan 2022 04:04:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 29 Jan 2022 04:04:44 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade36def3541e42ce15ffd1bf5ea1cc250cceb84a44de9f9d146e01deece7c4b`  
		Last Modified: Sat, 29 Jan 2022 04:06:52 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256b385799d95f1efdf26f2bc43addfdf0065556663579e9ff14558374cfc5e6`  
		Last Modified: Sat, 29 Jan 2022 04:07:26 GMT  
		Size: 63.7 MB (63654296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca46c14046a0a310dccae103438982827ebf0d5e184fc2958966363786623bd`  
		Last Modified: Sat, 29 Jan 2022 04:06:52 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acbbd623f5ce9237f9a46d32a7cd7651ebb72a38d2024e2000b7ab0909d1611`  
		Last Modified: Sat, 29 Jan 2022 04:06:52 GMT  
		Size: 1.8 KB (1822 bytes)  
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
