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
