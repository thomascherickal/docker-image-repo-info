## `vault:latest`

```console
$ docker pull vault@sha256:6d1b4c5a2a64efa6d5d3596fb25ef095f28e1f9d08c09a5814017081533b21d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:c5e0b81498f4859a499262acf895581b2151ebc7b7dcdb637eb00bb27551e5ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53139832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:423cb288c95d259a15b306576ab3ab9d527e499b005a08d4130fafe09f965ec0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:59 GMT
ADD file:a41bb436701fd0adf99a3157d19f172b3e54ea033f5c617009e2d1bdeac206d7 in / 
# Sat, 11 Feb 2023 04:46:59 GMT
CMD ["/bin/sh"]
# Tue, 07 Mar 2023 19:48:10 GMT
ARG VAULT_VERSION=1.13.0
# Tue, 07 Mar 2023 19:48:10 GMT
# ARGS: VAULT_VERSION=1.13.0
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 07 Mar 2023 19:48:18 GMT
# ARGS: VAULT_VERSION=1.13.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 07 Mar 2023 19:48:19 GMT
# ARGS: VAULT_VERSION=1.13.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 07 Mar 2023 19:48:19 GMT
VOLUME [/vault/logs]
# Tue, 07 Mar 2023 19:48:19 GMT
VOLUME [/vault/file]
# Tue, 07 Mar 2023 19:48:19 GMT
EXPOSE 8200
# Tue, 07 Mar 2023 19:48:19 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 07 Mar 2023 19:48:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Mar 2023 19:48:20 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:d261077062b2aebb9ca8dc61f2b00e7e2b4e44179d3cfbe526c4ee0c5e41b26f`  
		Last Modified: Sat, 11 Feb 2023 04:47:49 GMT  
		Size: 2.8 MB (2829633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14d31661d9bf68e3e8e5c7696b4bfdf8edabd2ab4d034193c322b693d806bc5`  
		Last Modified: Tue, 07 Mar 2023 19:49:13 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d542c976cfecd59eb1cb44c1922aca256fd75d2ae3e6458583eb9b9740c9ad`  
		Last Modified: Tue, 07 Mar 2023 19:49:21 GMT  
		Size: 50.3 MB (50306929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742781424743081d71cb716a95fbe6bf4cb68120d7d7c70de383aaf0cb783a58`  
		Last Modified: Tue, 07 Mar 2023 19:49:13 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da5ea6cd0c2b413819b368c606a1eeef7bde544c7a6acdeb41566973f19d89c`  
		Last Modified: Tue, 07 Mar 2023 19:49:13 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:28fd98af546be1665a4678c88260774c694e454fd015257449bf75330cec027c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50197917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f73f1f67a340bae759cdf70ed9284b31f8cf3274b9463bcef009bb7bf6de53d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:54 GMT
ADD file:767f6566ea2c075838c0a86ca644a37e446f309f68952f5f921970f046abd252 in / 
# Mon, 13 Mar 2023 16:12:54 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:07:47 GMT
ARG VAULT_VERSION=1.13.0
# Tue, 14 Mar 2023 01:07:47 GMT
# ARGS: VAULT_VERSION=1.13.0
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 14 Mar 2023 01:08:00 GMT
# ARGS: VAULT_VERSION=1.13.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 14 Mar 2023 01:08:01 GMT
# ARGS: VAULT_VERSION=1.13.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 14 Mar 2023 01:08:01 GMT
VOLUME [/vault/logs]
# Tue, 14 Mar 2023 01:08:01 GMT
VOLUME [/vault/file]
# Tue, 14 Mar 2023 01:08:01 GMT
EXPOSE 8200
# Tue, 14 Mar 2023 01:08:01 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 14 Mar 2023 01:08:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Mar 2023 01:08:02 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:7616dd32f4bf5fddffb2543afaac2355a5fc495348c01060cd67181e36343e96`  
		Last Modified: Fri, 10 Feb 2023 20:51:02 GMT  
		Size: 2.6 MB (2638152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1f485ff8e71a4c9555fadeb7fc26b8afa61b20dff5999ee89bc8c25001cee9`  
		Last Modified: Tue, 14 Mar 2023 01:09:13 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65e162950b9bf88b60c75819366e58b386b353c914fc6555de166911c603774`  
		Last Modified: Tue, 14 Mar 2023 01:09:22 GMT  
		Size: 47.6 MB (47556494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c181b282de46200743298dc51b928ce30a1899f8c3c6a2e59802dd295866b91c`  
		Last Modified: Tue, 14 Mar 2023 01:09:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3d143ba6962baa20993b8e518583e42bc1a52523112d5bfe2476453d6c94cc`  
		Last Modified: Tue, 14 Mar 2023 01:09:13 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:405a411f0d9eaf30c667f4c8355bcd537db30a13558f700c6e73c273f8f1ac4d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48962947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51306818dbce4efdbc437d66fefdbe69ca4d81f0417c20614fa9f0c84c1ce0af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:19 GMT
ADD file:50a841463966858f1c3ca87143cf96145d1d52f7349ef516adfbf21cdd5684fe in / 
# Fri, 10 Feb 2023 21:24:19 GMT
CMD ["/bin/sh"]
# Tue, 07 Mar 2023 19:09:07 GMT
ARG VAULT_VERSION=1.13.0
# Tue, 07 Mar 2023 19:09:07 GMT
# ARGS: VAULT_VERSION=1.13.0
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 07 Mar 2023 19:09:15 GMT
# ARGS: VAULT_VERSION=1.13.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 07 Mar 2023 19:09:16 GMT
# ARGS: VAULT_VERSION=1.13.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 07 Mar 2023 19:09:16 GMT
VOLUME [/vault/logs]
# Tue, 07 Mar 2023 19:09:16 GMT
VOLUME [/vault/file]
# Tue, 07 Mar 2023 19:09:16 GMT
EXPOSE 8200
# Tue, 07 Mar 2023 19:09:16 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 07 Mar 2023 19:09:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Mar 2023 19:09:17 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:6f0e733d82e26042c603e231c39b56abbabdad66673a736ec71c69c65be95f41`  
		Last Modified: Fri, 10 Feb 2023 21:25:10 GMT  
		Size: 2.7 MB (2725026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3a1f13beeed2834db1f1cfaf6d383325d5f58dc0fb56db3b77540615549cc2`  
		Last Modified: Tue, 07 Mar 2023 19:10:11 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fb88a3ba8fed11097e3414fc1abf54436e37f883824d1bce9c75e792449f01`  
		Last Modified: Tue, 07 Mar 2023 19:10:17 GMT  
		Size: 46.2 MB (46234652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273bacb9571802767a0f679e1d982123b12ddea2bfc0b34218770b8b861de379`  
		Last Modified: Tue, 07 Mar 2023 19:10:11 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78de7536ed89a538d88248bac9cb523f3d233a468af7be12eead7247497dd746`  
		Last Modified: Tue, 07 Mar 2023 19:10:11 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:79ae97ae93c7a22d3905f4ac71d2abb0e4f8fb6729f19aa2b8883914efb2bb9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.8 MB (49814173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcd5b3eb78704474285ac0727b81b74e409032432df54772c8761c126c599421`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:39 GMT
ADD file:d88c188553d983f16407f891790a4e553fda681fa265d89ec12a70ba2f41b0da in / 
# Fri, 10 Feb 2023 21:24:39 GMT
CMD ["/bin/sh"]
# Tue, 07 Mar 2023 18:41:45 GMT
ARG VAULT_VERSION=1.13.0
# Tue, 07 Mar 2023 18:41:46 GMT
# ARGS: VAULT_VERSION=1.13.0
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 07 Mar 2023 18:41:58 GMT
# ARGS: VAULT_VERSION=1.13.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 07 Mar 2023 18:41:59 GMT
# ARGS: VAULT_VERSION=1.13.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 07 Mar 2023 18:41:59 GMT
VOLUME [/vault/logs]
# Tue, 07 Mar 2023 18:41:59 GMT
VOLUME [/vault/file]
# Tue, 07 Mar 2023 18:41:59 GMT
EXPOSE 8200
# Tue, 07 Mar 2023 18:41:59 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 07 Mar 2023 18:41:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Mar 2023 18:41:59 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:84644bcd984e34c8b3bc44d8040b7017495e31100c1f4d726c92b40cf6cf7351`  
		Last Modified: Fri, 10 Feb 2023 21:25:51 GMT  
		Size: 2.8 MB (2835110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74b2418b8e5065a421a5fc22bc7bfa0ed8aa52cf28fc80048453dc5b300c477`  
		Last Modified: Tue, 07 Mar 2023 18:43:10 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf158ee032f749f870b059cc9e0a44378d5c8d53e5b85add30d251888f8beb78`  
		Last Modified: Tue, 07 Mar 2023 18:43:20 GMT  
		Size: 47.0 MB (46975790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e789f74989d4cc7bd1308265c54c892276cc18a848e3e52b1dc6f02ac508a8aa`  
		Last Modified: Tue, 07 Mar 2023 18:43:10 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6e6cfa4e994fe6232cd65d9c9df03ea2c54d4b8cdaf38b77f3022abc0ffc21`  
		Last Modified: Tue, 07 Mar 2023 18:43:10 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
