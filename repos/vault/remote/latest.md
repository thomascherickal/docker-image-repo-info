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
