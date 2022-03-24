<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:1.10.0`](#vault1100)
-	[`vault:1.7.10`](#vault1710)
-	[`vault:1.8.9`](#vault189)
-	[`vault:1.9.4`](#vault194)
-	[`vault:latest`](#vaultlatest)

## `vault:1.10.0`

```console
$ docker pull vault@sha256:37e2f51fa5da32462d373503f888a9665c9858437f6e25f53a0cfe74a7b5acb6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.10.0` - linux; amd64

```console
$ docker pull vault@sha256:cf915299a7a3372bea3e920f190c3b5e8a058f6cbdebf8c698edc6eef56608a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73959284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfc8c55968dfd0952942fa598f45752aaf2b061b1171e4b24c70e9ec5e7922a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 01:41:41 GMT
ARG VAULT_VERSION=1.10.0
# Thu, 24 Mar 2022 01:41:42 GMT
# ARGS: VAULT_VERSION=1.10.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 24 Mar 2022 01:41:50 GMT
# ARGS: VAULT_VERSION=1.10.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 24 Mar 2022 01:41:50 GMT
# ARGS: VAULT_VERSION=1.10.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 24 Mar 2022 01:41:51 GMT
VOLUME [/vault/logs]
# Thu, 24 Mar 2022 01:41:51 GMT
VOLUME [/vault/file]
# Thu, 24 Mar 2022 01:41:51 GMT
EXPOSE 8200
# Thu, 24 Mar 2022 01:41:51 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 24 Mar 2022 01:41:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 01:41:51 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fcd5c91b545b170c3df782b6f4d0fe2cc842f921a444d1f88d4ce4283e77fb`  
		Last Modified: Thu, 24 Mar 2022 01:42:06 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55650c8ff25aea687c7b9ed20f8a6c1c5f7a64797e9f77be32536d3a8b154c5c`  
		Last Modified: Thu, 24 Mar 2022 01:42:15 GMT  
		Size: 71.1 MB (71139845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49389f799b89b1f417ece330364ca79c08d5076386e03eefe19f06698df8cc70`  
		Last Modified: Thu, 24 Mar 2022 01:42:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052166a21f5a3e55f8f3791b0de5b332b3e52986826f9ce7af7a0f8707b6799a`  
		Last Modified: Thu, 24 Mar 2022 01:42:06 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.10.0` - linux; arm variant v6

```console
$ docker pull vault@sha256:ff1ef19640625e0d79c1d8f98a8ceeb39746a2c24a6ad88f094af7504f67fc0a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.3 MB (67258808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8d89b625bd58d87285c3f45346e132f8854fadbab24a9c2ed5fc0d49b3d34b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:33 GMT
ADD file:8f1611b9334907a82945fdb21e17ee41541ab95050fc199c60fca662759171a5 in / 
# Thu, 17 Mar 2022 14:32:33 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 02:17:08 GMT
ARG VAULT_VERSION=1.10.0
# Thu, 24 Mar 2022 02:17:10 GMT
# ARGS: VAULT_VERSION=1.10.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 24 Mar 2022 02:17:27 GMT
# ARGS: VAULT_VERSION=1.10.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 24 Mar 2022 02:17:29 GMT
# ARGS: VAULT_VERSION=1.10.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 24 Mar 2022 02:17:29 GMT
VOLUME [/vault/logs]
# Thu, 24 Mar 2022 02:17:30 GMT
VOLUME [/vault/file]
# Thu, 24 Mar 2022 02:17:30 GMT
EXPOSE 8200
# Thu, 24 Mar 2022 02:17:31 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 24 Mar 2022 02:17:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 02:17:31 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:4025825e6ef43541c3a3e1ecb0092bc1b098e792051c7e338d6da54f66b19661`  
		Last Modified: Thu, 17 Mar 2022 14:34:09 GMT  
		Size: 2.6 MB (2629364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5656a1d8b2ec3c83ee25e0b3e37ec024e00ea8f671bbb595f81dabfb14887149`  
		Last Modified: Thu, 24 Mar 2022 02:18:28 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1d87c0e6897e494054a23cbbedecd57d440ac5dc45a9117f66bc9a531d5277`  
		Last Modified: Thu, 24 Mar 2022 02:19:06 GMT  
		Size: 64.6 MB (64626175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0094c94ad85aecf5ea93c5628b4c9d3cbb341acabad0d66c42e72155d9a11f8`  
		Last Modified: Thu, 24 Mar 2022 02:18:28 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c02f66477cfed2edd7193ed81922e7c896ea0e95afe54e2700f2875d5f7977`  
		Last Modified: Thu, 24 Mar 2022 02:18:28 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.10.0` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:c0e7ef35040b72ecd41fad1582a8e5e6746302c4c37bd1820d7b51ef0dc8bf79
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69005318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f66d19936bb9c4bfac3fb587bb214d394314643156bac17bd3173253dbbdfbc8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 05:01:19 GMT
ARG VAULT_VERSION=1.10.0
# Thu, 24 Mar 2022 05:01:20 GMT
# ARGS: VAULT_VERSION=1.10.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 24 Mar 2022 05:01:28 GMT
# ARGS: VAULT_VERSION=1.10.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 24 Mar 2022 05:01:28 GMT
# ARGS: VAULT_VERSION=1.10.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 24 Mar 2022 05:01:29 GMT
VOLUME [/vault/logs]
# Thu, 24 Mar 2022 05:01:30 GMT
VOLUME [/vault/file]
# Thu, 24 Mar 2022 05:01:31 GMT
EXPOSE 8200
# Thu, 24 Mar 2022 05:01:33 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 24 Mar 2022 05:01:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:01:34 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0345d45f88ab1581e59610ee7c3e1fbcb18f0beca6c2ec3d38a6733d67be18`  
		Last Modified: Thu, 24 Mar 2022 05:02:04 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fbb2bd104f22a3cb2409e54521d5aaec2ec7681a992f0004725d35d017f8bf6`  
		Last Modified: Thu, 24 Mar 2022 05:02:12 GMT  
		Size: 66.3 MB (66286221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47eb2ed54a038e4f717ec7137afd45e52641967887e587ce919e9735ca1a4457`  
		Last Modified: Thu, 24 Mar 2022 05:02:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf50cb4d3613ef3733ece941d45994af7db2c98041f10b459f8a306d5495531`  
		Last Modified: Thu, 24 Mar 2022 05:02:04 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.10.0` - linux; 386

```console
$ docker pull vault@sha256:63f1b4a51d749000c7ffb169fc9c7bdf1f39f38f5717d65aa954d7278f2966ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70343920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a85611c60b4e96cfd50196109f8dc993598dde411f9194d3af844dff8ddf2145`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 23 Mar 2022 14:59:36 GMT
ADD file:5bb8a2cf301e0add52528df0f7f5c5b3c9b14495c5aa85c8fd628731fcd348aa in / 
# Wed, 23 Mar 2022 14:59:36 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 23:24:41 GMT
ARG VAULT_VERSION=1.10.0
# Wed, 23 Mar 2022 23:24:42 GMT
# ARGS: VAULT_VERSION=1.10.0
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 23 Mar 2022 23:24:51 GMT
# ARGS: VAULT_VERSION=1.10.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 23 Mar 2022 23:24:52 GMT
# ARGS: VAULT_VERSION=1.10.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 23 Mar 2022 23:24:53 GMT
VOLUME [/vault/logs]
# Wed, 23 Mar 2022 23:24:54 GMT
VOLUME [/vault/file]
# Wed, 23 Mar 2022 23:24:55 GMT
EXPOSE 8200
# Wed, 23 Mar 2022 23:24:57 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 23 Mar 2022 23:24:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 23:24:58 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:8fd9b2c548e42517da6865245538c8f53b774738b4fd7cb2d57ad8716e71748c`  
		Last Modified: Thu, 17 Mar 2022 16:35:25 GMT  
		Size: 2.8 MB (2823782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12151ac69da5960a9d37b274b82c9ce0a3d321e85dd2d09dea9bc0b0250f80c6`  
		Last Modified: Wed, 23 Mar 2022 23:26:21 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e80cf176f305c8da1eec389dafbd44a4da3f5170f76acb88ecc3277ff9ffa07`  
		Last Modified: Wed, 23 Mar 2022 23:26:29 GMT  
		Size: 67.5 MB (67516930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2e289666161b8d2e0af3be12b74ba2b1f17e972a6089cf78800b9b8c9da5d2`  
		Last Modified: Wed, 23 Mar 2022 23:26:21 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b78edfcbf8453e90aad203687e630c2fe98d0917710013ebe2249ac3adf943`  
		Last Modified: Wed, 23 Mar 2022 23:26:21 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.7.10`

```console
$ docker pull vault@sha256:5f8db9add562a13bcf7fd34e19ce342210ad3a5422b12322f7fa2851b7f96821
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.7.10` - linux; amd64

```console
$ docker pull vault@sha256:fd1bd1eaa4f5fa63b5c786688a0053732bc87a447328196c0b9ec64720883f95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68116759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a06826f2eccb8617b2f9abf3deb2a9378272e4fbb2fb71254b6ae33165488e7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 06:09:57 GMT
ARG VAULT_VERSION=1.7.10
# Fri, 18 Mar 2022 06:09:58 GMT
# ARGS: VAULT_VERSION=1.7.10
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 18 Mar 2022 06:10:06 GMT
# ARGS: VAULT_VERSION=1.7.10
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 18 Mar 2022 06:10:07 GMT
# ARGS: VAULT_VERSION=1.7.10
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 18 Mar 2022 06:10:07 GMT
VOLUME [/vault/logs]
# Fri, 18 Mar 2022 06:10:08 GMT
VOLUME [/vault/file]
# Fri, 18 Mar 2022 06:10:08 GMT
EXPOSE 8200
# Fri, 18 Mar 2022 06:10:08 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 18 Mar 2022 06:10:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 06:10:08 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4b9537c027109ec19372dc29ed2b3f279b0bbd625d554a1f798794e1601e4`  
		Last Modified: Fri, 18 Mar 2022 06:11:15 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6350df29b1eff600e4f6afa14109a626df1a2659e4755f37ffdfe55f49998fb`  
		Last Modified: Fri, 18 Mar 2022 06:11:27 GMT  
		Size: 65.3 MB (65297320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3322187b1172f7634af6e3df6cd08eb084437fe9acd38ba5e2799a07ded461`  
		Last Modified: Fri, 18 Mar 2022 06:11:15 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ad62b825dd56132c58906d824f919055c7192e66205b090cd49b2c9a47787f`  
		Last Modified: Fri, 18 Mar 2022 06:11:15 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.7.10` - linux; arm variant v6

```console
$ docker pull vault@sha256:f6b12d003ee8ab9315dfc7cd6fb485f02ab1438edaf437b6065a9251c148d172
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.9 MB (62854071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22bf530236bd5594a8639627bb8c2fc5d8bd1e95bbcb1f429a16907db124595f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:33 GMT
ADD file:8f1611b9334907a82945fdb21e17ee41541ab95050fc199c60fca662759171a5 in / 
# Thu, 17 Mar 2022 14:32:33 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:09:09 GMT
ARG VAULT_VERSION=1.7.10
# Thu, 17 Mar 2022 18:09:10 GMT
# ARGS: VAULT_VERSION=1.7.10
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 17 Mar 2022 18:09:26 GMT
# ARGS: VAULT_VERSION=1.7.10
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 17 Mar 2022 18:09:28 GMT
# ARGS: VAULT_VERSION=1.7.10
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 17 Mar 2022 18:09:28 GMT
VOLUME [/vault/logs]
# Thu, 17 Mar 2022 18:09:28 GMT
VOLUME [/vault/file]
# Thu, 17 Mar 2022 18:09:29 GMT
EXPOSE 8200
# Thu, 17 Mar 2022 18:09:29 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Mar 2022 18:09:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 18:09:30 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:4025825e6ef43541c3a3e1ecb0092bc1b098e792051c7e338d6da54f66b19661`  
		Last Modified: Thu, 17 Mar 2022 14:34:09 GMT  
		Size: 2.6 MB (2629364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59ca238ef24d6d7a96d4b74bf29cc0de756651059f2375d3fa0dcade75e1a3b`  
		Last Modified: Thu, 17 Mar 2022 18:12:17 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c003beaa256153fcb0d8cf0328370e4ca4f272df41e7293058d9fe18e648e3`  
		Last Modified: Thu, 17 Mar 2022 18:12:49 GMT  
		Size: 60.2 MB (60221436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1876404e7888c9bd41809848aff4b865aa5970a61fef87ec6f4d491fc2e64b17`  
		Last Modified: Thu, 17 Mar 2022 18:12:17 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f9c1b71631ef750ee029b9670d29fcf43aceb4cd96e833b33574d5c554c827`  
		Last Modified: Thu, 17 Mar 2022 18:12:17 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.7.10` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:53137247125158276c533bf3ddb44fe68b0b935c08e14e71f1c416e996b463e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.5 MB (64536945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d4ad691c6711e4cf1656ee244175a32f2d13201600e5a6fb22b48d491adc9bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 21:22:11 GMT
ARG VAULT_VERSION=1.7.10
# Thu, 17 Mar 2022 21:22:12 GMT
# ARGS: VAULT_VERSION=1.7.10
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 17 Mar 2022 21:22:19 GMT
# ARGS: VAULT_VERSION=1.7.10
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 17 Mar 2022 21:22:19 GMT
# ARGS: VAULT_VERSION=1.7.10
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 17 Mar 2022 21:22:20 GMT
VOLUME [/vault/logs]
# Thu, 17 Mar 2022 21:22:21 GMT
VOLUME [/vault/file]
# Thu, 17 Mar 2022 21:22:22 GMT
EXPOSE 8200
# Thu, 17 Mar 2022 21:22:24 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Mar 2022 21:22:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 21:22:25 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd13d7d106c122c0a4a4a5ed9ff61dcf8754710ea5dc3638602df45a6693066`  
		Last Modified: Thu, 17 Mar 2022 21:23:39 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40cce72deac51a902601afc78ca35aae6a7205df390e537fde3e2910dc042ce`  
		Last Modified: Thu, 17 Mar 2022 21:23:48 GMT  
		Size: 61.8 MB (61817852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4892bdea507ec04abe9984bc4e0376203aa8b9fb2823dfd0eea4342083b1c71a`  
		Last Modified: Thu, 17 Mar 2022 21:23:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4de0c9398f7d24c114c8e074d91da860bc835ad2da8976f831dffcd8d886d96`  
		Last Modified: Thu, 17 Mar 2022 21:23:39 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.7.10` - linux; 386

```console
$ docker pull vault@sha256:75d2e28898341fff94b8e5560c4db2a8ac38a659a8aa406978aa83dfb4316b7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (65979134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c0da6169547e68c341d683cbdb4032b62647882dfed4d1c5cb53e7aaad8ec47`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 23 Mar 2022 14:59:36 GMT
ADD file:5bb8a2cf301e0add52528df0f7f5c5b3c9b14495c5aa85c8fd628731fcd348aa in / 
# Wed, 23 Mar 2022 14:59:36 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 23:25:46 GMT
ARG VAULT_VERSION=1.7.10
# Wed, 23 Mar 2022 23:25:47 GMT
# ARGS: VAULT_VERSION=1.7.10
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 23 Mar 2022 23:25:54 GMT
# ARGS: VAULT_VERSION=1.7.10
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 23 Mar 2022 23:25:55 GMT
# ARGS: VAULT_VERSION=1.7.10
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 23 Mar 2022 23:25:56 GMT
VOLUME [/vault/logs]
# Wed, 23 Mar 2022 23:25:57 GMT
VOLUME [/vault/file]
# Wed, 23 Mar 2022 23:25:58 GMT
EXPOSE 8200
# Wed, 23 Mar 2022 23:26:00 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 23 Mar 2022 23:26:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 23:26:01 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:8fd9b2c548e42517da6865245538c8f53b774738b4fd7cb2d57ad8716e71748c`  
		Last Modified: Thu, 17 Mar 2022 16:35:25 GMT  
		Size: 2.8 MB (2823782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8182a5546007f0b698e7c85ea8981bef80d528792b359469a5531472d3b46db5`  
		Last Modified: Wed, 23 Mar 2022 23:27:14 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e14e99e5b03f9e728b188b1cda9ac2c035bcd66136f214cbc94313ce5d7285`  
		Last Modified: Wed, 23 Mar 2022 23:27:27 GMT  
		Size: 63.2 MB (63152143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e88985d75c7c1c63f364a66ea50c51ac9b6688abd9dc380c6136541e3a66a3`  
		Last Modified: Wed, 23 Mar 2022 23:27:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a79846c360202ebbaf75a9c849fb0d0211bb9faf776df64c9b079bef33a81f`  
		Last Modified: Wed, 23 Mar 2022 23:27:14 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.8.9`

```console
$ docker pull vault@sha256:c170f7c8565d4400e219b321edfcc1a68a496627aa2b037ee1c518231ae5c771
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.8.9` - linux; amd64

```console
$ docker pull vault@sha256:8a0a62d51cfa0ad57de4c6bc6bc9ad671ecc3547bb9596d152a8f7780d40ac6b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70592291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00c3b4d5f8e8cb595d55119cb6d080d4df0a99bba12326f737cd5f11e25a2d88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 06:09:40 GMT
ARG VAULT_VERSION=1.8.9
# Fri, 18 Mar 2022 06:09:41 GMT
# ARGS: VAULT_VERSION=1.8.9
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 18 Mar 2022 06:09:51 GMT
# ARGS: VAULT_VERSION=1.8.9
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 18 Mar 2022 06:09:52 GMT
# ARGS: VAULT_VERSION=1.8.9
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 18 Mar 2022 06:09:52 GMT
VOLUME [/vault/logs]
# Fri, 18 Mar 2022 06:09:52 GMT
VOLUME [/vault/file]
# Fri, 18 Mar 2022 06:09:52 GMT
EXPOSE 8200
# Fri, 18 Mar 2022 06:09:53 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 18 Mar 2022 06:09:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 06:09:53 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4099bee20305be9d397f0a5f16cdc708ee6f346b69a29411e6b6526fb765a0b2`  
		Last Modified: Fri, 18 Mar 2022 06:10:57 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c97522e2613d3a3e3b29f19b8982271d578b04887f6502f5164c4a7409d04da`  
		Last Modified: Fri, 18 Mar 2022 06:11:07 GMT  
		Size: 67.8 MB (67772854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7dad1471df7bbcddf38caa50e76d6d746261a0c8b775d10c0e94c5721eeb86`  
		Last Modified: Fri, 18 Mar 2022 06:10:57 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8600c16ab1de1a99e8114607ce920907e00234899669f55288f87a0c5947c3a`  
		Last Modified: Fri, 18 Mar 2022 06:10:57 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.8.9` - linux; arm variant v6

```console
$ docker pull vault@sha256:58000bd3048e2c54f2362a56fac93d42cc64acc6945c976268de5cb3ec20c3f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64946593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f489b7f54783ec2f8d905793544fc4347730780fc77887e01fb6646a6ffc5039`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:33 GMT
ADD file:8f1611b9334907a82945fdb21e17ee41541ab95050fc199c60fca662759171a5 in / 
# Thu, 17 Mar 2022 14:32:33 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:08:36 GMT
ARG VAULT_VERSION=1.8.9
# Thu, 17 Mar 2022 18:08:37 GMT
# ARGS: VAULT_VERSION=1.8.9
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 17 Mar 2022 18:08:53 GMT
# ARGS: VAULT_VERSION=1.8.9
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 17 Mar 2022 18:08:55 GMT
# ARGS: VAULT_VERSION=1.8.9
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 17 Mar 2022 18:08:55 GMT
VOLUME [/vault/logs]
# Thu, 17 Mar 2022 18:08:56 GMT
VOLUME [/vault/file]
# Thu, 17 Mar 2022 18:08:56 GMT
EXPOSE 8200
# Thu, 17 Mar 2022 18:08:57 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Mar 2022 18:08:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 18:08:57 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:4025825e6ef43541c3a3e1ecb0092bc1b098e792051c7e338d6da54f66b19661`  
		Last Modified: Thu, 17 Mar 2022 14:34:09 GMT  
		Size: 2.6 MB (2629364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49973ed8eba6a988b1f3be1693c13c9a3367807431d814c99782b86bf6c98b08`  
		Last Modified: Thu, 17 Mar 2022 18:11:37 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0204a11a4a18d4933ff7097b25306191457f0e7c1761d5a305524b1631498725`  
		Last Modified: Thu, 17 Mar 2022 18:12:10 GMT  
		Size: 62.3 MB (62313960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e6de87910606c0704b88cb82cbdfff7a8061c9cecbe42224253a027528b45d`  
		Last Modified: Thu, 17 Mar 2022 18:11:37 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc28e894eac02c733cfa4210884f8676fa2a6fecce13404d7f178b247c54faa7`  
		Last Modified: Thu, 17 Mar 2022 18:11:37 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.8.9` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:69196905f039bbc53826c5ad24b31640596074ce101a067768510c5e14e79413
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66858763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2abf260c24fe32eb22d4f30cd1a692b421c6cefb14b8933eb507eec2d990f5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 21:21:51 GMT
ARG VAULT_VERSION=1.8.9
# Thu, 17 Mar 2022 21:21:52 GMT
# ARGS: VAULT_VERSION=1.8.9
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 17 Mar 2022 21:21:59 GMT
# ARGS: VAULT_VERSION=1.8.9
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 17 Mar 2022 21:22:00 GMT
# ARGS: VAULT_VERSION=1.8.9
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 17 Mar 2022 21:22:01 GMT
VOLUME [/vault/logs]
# Thu, 17 Mar 2022 21:22:02 GMT
VOLUME [/vault/file]
# Thu, 17 Mar 2022 21:22:03 GMT
EXPOSE 8200
# Thu, 17 Mar 2022 21:22:05 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Mar 2022 21:22:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 21:22:06 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a7297336d7f661e2b659153d30784ff7446d75cbf52d4d284c3160d403f3c7`  
		Last Modified: Thu, 17 Mar 2022 21:23:22 GMT  
		Size: 1.2 KB (1237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b17be52b002a15336d2f31c3570c074b0da159439b478027ff22ac0f2179ab92`  
		Last Modified: Thu, 17 Mar 2022 21:23:31 GMT  
		Size: 64.1 MB (64139672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c066f87390fa8fa57be11b522737e5dd4ebcd550c429d561e538631dc42c1501`  
		Last Modified: Thu, 17 Mar 2022 21:23:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaeba50cc34a51c09edbf6b157f728539d38ac5a231c45b16d80eb9ff934d38`  
		Last Modified: Thu, 17 Mar 2022 21:23:22 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.8.9` - linux; 386

```console
$ docker pull vault@sha256:abf84ebd812fc6d466bd67240fdee2742925c57ed1fcd1e39db21610c7014abb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68314347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c710daeae88a4e594097d305444360f88fc2ca2c3d30d48361e63506038adb0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 23 Mar 2022 14:59:36 GMT
ADD file:5bb8a2cf301e0add52528df0f7f5c5b3c9b14495c5aa85c8fd628731fcd348aa in / 
# Wed, 23 Mar 2022 14:59:36 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 23:25:26 GMT
ARG VAULT_VERSION=1.8.9
# Wed, 23 Mar 2022 23:25:27 GMT
# ARGS: VAULT_VERSION=1.8.9
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 23 Mar 2022 23:25:35 GMT
# ARGS: VAULT_VERSION=1.8.9
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 23 Mar 2022 23:25:35 GMT
# ARGS: VAULT_VERSION=1.8.9
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 23 Mar 2022 23:25:36 GMT
VOLUME [/vault/logs]
# Wed, 23 Mar 2022 23:25:37 GMT
VOLUME [/vault/file]
# Wed, 23 Mar 2022 23:25:38 GMT
EXPOSE 8200
# Wed, 23 Mar 2022 23:25:40 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 23 Mar 2022 23:25:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 23:25:41 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:8fd9b2c548e42517da6865245538c8f53b774738b4fd7cb2d57ad8716e71748c`  
		Last Modified: Thu, 17 Mar 2022 16:35:25 GMT  
		Size: 2.8 MB (2823782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941ef7055180da17d9f847f836fc70c1fb1485ead2bc020c25c039e2e0b663a7`  
		Last Modified: Wed, 23 Mar 2022 23:26:58 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e61bca97ea5c9c6686742e820aeb76a9d3dcc97775d379c84052259e280a31`  
		Last Modified: Wed, 23 Mar 2022 23:27:05 GMT  
		Size: 65.5 MB (65487359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ed7d3829747490b292ce267d6cfd7c64766cfe5ff20c96bf7736a193381b7c`  
		Last Modified: Wed, 23 Mar 2022 23:26:58 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7685edce2baff5a31aeb4ee6be8f4924ad5130d9021716cebbd366377385d00`  
		Last Modified: Wed, 23 Mar 2022 23:26:58 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.9.4`

```console
$ docker pull vault@sha256:cecb88ecdbbe0e2bd385ab0d61aa62be0899441c78757b28dc093b88ec15f61b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.9.4` - linux; amd64

```console
$ docker pull vault@sha256:2f69ca64144ed051fce5c56662275638018ccc8abdca36c081c7d8d13c6e5eef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73148656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ea101960f4b2ee058f5c271c8648638fe99681f35a4e7e93e17afe6464f726b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 06:09:23 GMT
ARG VAULT_VERSION=1.9.4
# Fri, 18 Mar 2022 06:09:23 GMT
# ARGS: VAULT_VERSION=1.9.4
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 18 Mar 2022 06:09:33 GMT
# ARGS: VAULT_VERSION=1.9.4
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 18 Mar 2022 06:09:34 GMT
# ARGS: VAULT_VERSION=1.9.4
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 18 Mar 2022 06:09:34 GMT
VOLUME [/vault/logs]
# Fri, 18 Mar 2022 06:09:34 GMT
VOLUME [/vault/file]
# Fri, 18 Mar 2022 06:09:34 GMT
EXPOSE 8200
# Fri, 18 Mar 2022 06:09:35 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 18 Mar 2022 06:09:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 06:09:35 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b0c57e7bd2053caa92e6d1a842e92613d7e03acae03b8c01599696c8a4618f`  
		Last Modified: Fri, 18 Mar 2022 06:10:38 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9151986c9e0e51544b8aa0381d6c3a7fddde89ef20da9da6922b4b7c79e6fab4`  
		Last Modified: Fri, 18 Mar 2022 06:10:47 GMT  
		Size: 70.3 MB (70329219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eafa7257e3b0259d6322d1cec41b4c0d06963cf88f7f79e67f21c5307ad0b94`  
		Last Modified: Fri, 18 Mar 2022 06:10:38 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1319691e2a6f384311de3d4e49fd05106b3ea45c75bbc1749dc61ad4dd9de9af`  
		Last Modified: Fri, 18 Mar 2022 06:10:38 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.9.4` - linux; arm variant v6

```console
$ docker pull vault@sha256:8b916a4987068de93aab60ee54df21cad03be4a7324da4a2c0161d5cc60d63b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66494186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2550cb1d7a7c48b3066fd8863eb81242f216dafdd7a55aaba071644875364440`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:33 GMT
ADD file:8f1611b9334907a82945fdb21e17ee41541ab95050fc199c60fca662759171a5 in / 
# Thu, 17 Mar 2022 14:32:33 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:08:03 GMT
ARG VAULT_VERSION=1.9.4
# Thu, 17 Mar 2022 18:08:04 GMT
# ARGS: VAULT_VERSION=1.9.4
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 17 Mar 2022 18:08:20 GMT
# ARGS: VAULT_VERSION=1.9.4
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 17 Mar 2022 18:08:22 GMT
# ARGS: VAULT_VERSION=1.9.4
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 17 Mar 2022 18:08:22 GMT
VOLUME [/vault/logs]
# Thu, 17 Mar 2022 18:08:23 GMT
VOLUME [/vault/file]
# Thu, 17 Mar 2022 18:08:23 GMT
EXPOSE 8200
# Thu, 17 Mar 2022 18:08:24 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Mar 2022 18:08:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 18:08:25 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:4025825e6ef43541c3a3e1ecb0092bc1b098e792051c7e338d6da54f66b19661`  
		Last Modified: Thu, 17 Mar 2022 14:34:09 GMT  
		Size: 2.6 MB (2629364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ade8edc768b3c78703afae802967606e4f00d8d0a1c819acb5e536f4c60c485`  
		Last Modified: Thu, 17 Mar 2022 18:10:50 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ed5243b3ecfe07eff72832d3f23d64e0711108c8e0d37d5551c3901d99b37f`  
		Last Modified: Thu, 17 Mar 2022 18:11:26 GMT  
		Size: 63.9 MB (63861549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a367589cedf81ccafa3913ba590851ada5b32cd82345d1b72ff211c8ec92f5`  
		Last Modified: Thu, 17 Mar 2022 18:10:50 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665661b81f302cf4b9b7d7d60a5909b93e6a477bd94e5d70d3f1dd8618bff3a6`  
		Last Modified: Thu, 17 Mar 2022 18:10:50 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.9.4` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:5f9d8e975f8a84c4ec936a26226a8e671187d9aab7b18cc68e58e340e2c1258e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68259983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e27c250705bc5e11453057b1e017074f7d58d6ca093de25edd4e1c062b14b526`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 21:21:32 GMT
ARG VAULT_VERSION=1.9.4
# Thu, 17 Mar 2022 21:21:33 GMT
# ARGS: VAULT_VERSION=1.9.4
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 17 Mar 2022 21:21:40 GMT
# ARGS: VAULT_VERSION=1.9.4
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 17 Mar 2022 21:21:41 GMT
# ARGS: VAULT_VERSION=1.9.4
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 17 Mar 2022 21:21:41 GMT
VOLUME [/vault/logs]
# Thu, 17 Mar 2022 21:21:42 GMT
VOLUME [/vault/file]
# Thu, 17 Mar 2022 21:21:43 GMT
EXPOSE 8200
# Thu, 17 Mar 2022 21:21:45 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Mar 2022 21:21:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 21:21:46 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b8311591d8ad7007a6ab76dcc2338e5e055311f99f30641b7e15bb6a2d7bfb`  
		Last Modified: Thu, 17 Mar 2022 21:23:00 GMT  
		Size: 1.2 KB (1237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf62ddb38aff6e05f3c9a71f3a0fb9c399c8ceb23f2fc282067f27883caa447`  
		Last Modified: Thu, 17 Mar 2022 21:23:10 GMT  
		Size: 65.5 MB (65540890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88aebca7138380de1e56351f1983f4ca1e79abfb20b3323a0917b98be30aa93`  
		Last Modified: Thu, 17 Mar 2022 21:23:00 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2253c5b1e2bcefc0c5c9c0054f18ba791cf5cba954d4f568a7955899bf18384f`  
		Last Modified: Thu, 17 Mar 2022 21:23:00 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.9.4` - linux; 386

```console
$ docker pull vault@sha256:36b7666aa72eb510ebb4a8cb9aacdeb3d203d831f392f0829c274d474145c1ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69535447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5821fd5ea766408879eb713bf26d8eecd28129d40dafd2f835c7d570f1785634`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 23 Mar 2022 14:59:36 GMT
ADD file:5bb8a2cf301e0add52528df0f7f5c5b3c9b14495c5aa85c8fd628731fcd348aa in / 
# Wed, 23 Mar 2022 14:59:36 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 23:25:04 GMT
ARG VAULT_VERSION=1.9.4
# Wed, 23 Mar 2022 23:25:05 GMT
# ARGS: VAULT_VERSION=1.9.4
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 23 Mar 2022 23:25:13 GMT
# ARGS: VAULT_VERSION=1.9.4
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 23 Mar 2022 23:25:14 GMT
# ARGS: VAULT_VERSION=1.9.4
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 23 Mar 2022 23:25:14 GMT
VOLUME [/vault/logs]
# Wed, 23 Mar 2022 23:25:15 GMT
VOLUME [/vault/file]
# Wed, 23 Mar 2022 23:25:16 GMT
EXPOSE 8200
# Wed, 23 Mar 2022 23:25:18 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 23 Mar 2022 23:25:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 23:25:19 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:8fd9b2c548e42517da6865245538c8f53b774738b4fd7cb2d57ad8716e71748c`  
		Last Modified: Thu, 17 Mar 2022 16:35:25 GMT  
		Size: 2.8 MB (2823782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981f36b9a5d0538c8f00c2b64b9f3edc73b3a788459d23cbb465337eb9b06835`  
		Last Modified: Wed, 23 Mar 2022 23:26:41 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fd2cdd60ecb609abe77a464612b4c27fafd663e125cebb2381594347108ce0`  
		Last Modified: Wed, 23 Mar 2022 23:26:50 GMT  
		Size: 66.7 MB (66708460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ff3d238e8dcaebc75e0fa55a22bc243a4f6847b25c8eaf988abf0f5c1bb367`  
		Last Modified: Wed, 23 Mar 2022 23:26:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b38295ce26c64f2e651dfa5ede3862c59f2a0e429ba72e8492c423e49a9b36d`  
		Last Modified: Wed, 23 Mar 2022 23:26:41 GMT  
		Size: 1.8 KB (1810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:latest`

```console
$ docker pull vault@sha256:37e2f51fa5da32462d373503f888a9665c9858437f6e25f53a0cfe74a7b5acb6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:cf915299a7a3372bea3e920f190c3b5e8a058f6cbdebf8c698edc6eef56608a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73959284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfc8c55968dfd0952942fa598f45752aaf2b061b1171e4b24c70e9ec5e7922a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 01:41:41 GMT
ARG VAULT_VERSION=1.10.0
# Thu, 24 Mar 2022 01:41:42 GMT
# ARGS: VAULT_VERSION=1.10.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 24 Mar 2022 01:41:50 GMT
# ARGS: VAULT_VERSION=1.10.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 24 Mar 2022 01:41:50 GMT
# ARGS: VAULT_VERSION=1.10.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 24 Mar 2022 01:41:51 GMT
VOLUME [/vault/logs]
# Thu, 24 Mar 2022 01:41:51 GMT
VOLUME [/vault/file]
# Thu, 24 Mar 2022 01:41:51 GMT
EXPOSE 8200
# Thu, 24 Mar 2022 01:41:51 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 24 Mar 2022 01:41:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 01:41:51 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fcd5c91b545b170c3df782b6f4d0fe2cc842f921a444d1f88d4ce4283e77fb`  
		Last Modified: Thu, 24 Mar 2022 01:42:06 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55650c8ff25aea687c7b9ed20f8a6c1c5f7a64797e9f77be32536d3a8b154c5c`  
		Last Modified: Thu, 24 Mar 2022 01:42:15 GMT  
		Size: 71.1 MB (71139845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49389f799b89b1f417ece330364ca79c08d5076386e03eefe19f06698df8cc70`  
		Last Modified: Thu, 24 Mar 2022 01:42:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052166a21f5a3e55f8f3791b0de5b332b3e52986826f9ce7af7a0f8707b6799a`  
		Last Modified: Thu, 24 Mar 2022 01:42:06 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:ff1ef19640625e0d79c1d8f98a8ceeb39746a2c24a6ad88f094af7504f67fc0a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.3 MB (67258808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8d89b625bd58d87285c3f45346e132f8854fadbab24a9c2ed5fc0d49b3d34b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:33 GMT
ADD file:8f1611b9334907a82945fdb21e17ee41541ab95050fc199c60fca662759171a5 in / 
# Thu, 17 Mar 2022 14:32:33 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 02:17:08 GMT
ARG VAULT_VERSION=1.10.0
# Thu, 24 Mar 2022 02:17:10 GMT
# ARGS: VAULT_VERSION=1.10.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 24 Mar 2022 02:17:27 GMT
# ARGS: VAULT_VERSION=1.10.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 24 Mar 2022 02:17:29 GMT
# ARGS: VAULT_VERSION=1.10.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 24 Mar 2022 02:17:29 GMT
VOLUME [/vault/logs]
# Thu, 24 Mar 2022 02:17:30 GMT
VOLUME [/vault/file]
# Thu, 24 Mar 2022 02:17:30 GMT
EXPOSE 8200
# Thu, 24 Mar 2022 02:17:31 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 24 Mar 2022 02:17:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 02:17:31 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:4025825e6ef43541c3a3e1ecb0092bc1b098e792051c7e338d6da54f66b19661`  
		Last Modified: Thu, 17 Mar 2022 14:34:09 GMT  
		Size: 2.6 MB (2629364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5656a1d8b2ec3c83ee25e0b3e37ec024e00ea8f671bbb595f81dabfb14887149`  
		Last Modified: Thu, 24 Mar 2022 02:18:28 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1d87c0e6897e494054a23cbbedecd57d440ac5dc45a9117f66bc9a531d5277`  
		Last Modified: Thu, 24 Mar 2022 02:19:06 GMT  
		Size: 64.6 MB (64626175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0094c94ad85aecf5ea93c5628b4c9d3cbb341acabad0d66c42e72155d9a11f8`  
		Last Modified: Thu, 24 Mar 2022 02:18:28 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c02f66477cfed2edd7193ed81922e7c896ea0e95afe54e2700f2875d5f7977`  
		Last Modified: Thu, 24 Mar 2022 02:18:28 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:c0e7ef35040b72ecd41fad1582a8e5e6746302c4c37bd1820d7b51ef0dc8bf79
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69005318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f66d19936bb9c4bfac3fb587bb214d394314643156bac17bd3173253dbbdfbc8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 05:01:19 GMT
ARG VAULT_VERSION=1.10.0
# Thu, 24 Mar 2022 05:01:20 GMT
# ARGS: VAULT_VERSION=1.10.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 24 Mar 2022 05:01:28 GMT
# ARGS: VAULT_VERSION=1.10.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 24 Mar 2022 05:01:28 GMT
# ARGS: VAULT_VERSION=1.10.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 24 Mar 2022 05:01:29 GMT
VOLUME [/vault/logs]
# Thu, 24 Mar 2022 05:01:30 GMT
VOLUME [/vault/file]
# Thu, 24 Mar 2022 05:01:31 GMT
EXPOSE 8200
# Thu, 24 Mar 2022 05:01:33 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 24 Mar 2022 05:01:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:01:34 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0345d45f88ab1581e59610ee7c3e1fbcb18f0beca6c2ec3d38a6733d67be18`  
		Last Modified: Thu, 24 Mar 2022 05:02:04 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fbb2bd104f22a3cb2409e54521d5aaec2ec7681a992f0004725d35d017f8bf6`  
		Last Modified: Thu, 24 Mar 2022 05:02:12 GMT  
		Size: 66.3 MB (66286221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47eb2ed54a038e4f717ec7137afd45e52641967887e587ce919e9735ca1a4457`  
		Last Modified: Thu, 24 Mar 2022 05:02:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf50cb4d3613ef3733ece941d45994af7db2c98041f10b459f8a306d5495531`  
		Last Modified: Thu, 24 Mar 2022 05:02:04 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:63f1b4a51d749000c7ffb169fc9c7bdf1f39f38f5717d65aa954d7278f2966ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70343920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a85611c60b4e96cfd50196109f8dc993598dde411f9194d3af844dff8ddf2145`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 23 Mar 2022 14:59:36 GMT
ADD file:5bb8a2cf301e0add52528df0f7f5c5b3c9b14495c5aa85c8fd628731fcd348aa in / 
# Wed, 23 Mar 2022 14:59:36 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 23:24:41 GMT
ARG VAULT_VERSION=1.10.0
# Wed, 23 Mar 2022 23:24:42 GMT
# ARGS: VAULT_VERSION=1.10.0
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 23 Mar 2022 23:24:51 GMT
# ARGS: VAULT_VERSION=1.10.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 23 Mar 2022 23:24:52 GMT
# ARGS: VAULT_VERSION=1.10.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 23 Mar 2022 23:24:53 GMT
VOLUME [/vault/logs]
# Wed, 23 Mar 2022 23:24:54 GMT
VOLUME [/vault/file]
# Wed, 23 Mar 2022 23:24:55 GMT
EXPOSE 8200
# Wed, 23 Mar 2022 23:24:57 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 23 Mar 2022 23:24:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 23:24:58 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:8fd9b2c548e42517da6865245538c8f53b774738b4fd7cb2d57ad8716e71748c`  
		Last Modified: Thu, 17 Mar 2022 16:35:25 GMT  
		Size: 2.8 MB (2823782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12151ac69da5960a9d37b274b82c9ce0a3d321e85dd2d09dea9bc0b0250f80c6`  
		Last Modified: Wed, 23 Mar 2022 23:26:21 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e80cf176f305c8da1eec389dafbd44a4da3f5170f76acb88ecc3277ff9ffa07`  
		Last Modified: Wed, 23 Mar 2022 23:26:29 GMT  
		Size: 67.5 MB (67516930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2e289666161b8d2e0af3be12b74ba2b1f17e972a6089cf78800b9b8c9da5d2`  
		Last Modified: Wed, 23 Mar 2022 23:26:21 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b78edfcbf8453e90aad203687e630c2fe98d0917710013ebe2249ac3adf943`  
		Last Modified: Wed, 23 Mar 2022 23:26:21 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
